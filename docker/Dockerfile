FROM python:3.8

WORKDIR /python_bar_review
COPY ./Pipfile Pipfile
COPY ./Pipfile.lock Pipfile.lock

RUN apt-get update -y && apt-get install python3-pip -y && pip3 install pip --upgrade && apt-get clean
RUN apt-get install -y  gcc gfortran python-dev libopenblas-dev liblapack-dev cython
RUN pip install pipenv
RUN pipenv install --system

RUN curl -sL https://deb.nodesource.com/setup_12.x | bash -
RUN apt-get install -y nodejs

RUN jupyter labextension install @jupyterlab/toc
RUN jupyter labextension install @jupyter-widgets/jupyterlab-manager
RUN jupyter labextension install jupyter-matplotlib
RUN jupyter labextension install @krassowski/jupyterlab_go_to_definition

EXPOSE 8080

CMD pipenv run jupyter lab --ip=0.0.0.0 --port=8080 --allow-root

FROM python:3.7

WORKDIR /python_bar_review
COPY ./Pipfile Pipfile
COPY ./Pipfile.lock Pipfile.lock

RUN pip install pipenv
RUN pipenv install --system

EXPOSE 8080

CMD pipenv run jupyter notebook --ip=0.0.0.0 --port=8080 --allow-root

# Python. Bar Review

![Python Bar Review](img/promo.png)

Набор заметок о синтаксисе языка Python.
Каждая заметка — отдельный [Jupyter notebook](https://jupyter.org).
Содержимое ноутбуков можно смотреть по ссылке [https://ckorikov.github.io/python-bar-review/](https://ckorikov.github.io/python-bar-review/). Для интерактивного просмотра нужен Jupyter.

## Содержание

1. [Вложенные функции, замыкания и декораторы](01-nested_functions-closures-decorators.ipynb)
2. [Итераторы, генераторы и функциональное программирование](02-iterators-generators-functional_programming.ipynb)
3. [Контейнеры 1](03-containers-1.ipynb)
4. [Контейнеры 2](04-containers-2.ipynb)

В работе:

- [ ] [Конкурентное программирование — WIP](05-concurrency.ipynb)
- [ ] [Моржовый оператор и новинки python 3.8 — WIP](06-walrus_operator_and_3p8.ipynb)
- [ ] [Алгоритмы. Числа — WIP](xx-algorithms-numbers.ipynb)
- [ ] [Алгоритмы. ML — WIP](xx-algorithms-machine_learning.ipynb)

## Идеи для занятий (файл может меняться)

<img src="syllabus/syllabus.png" width="100%"/>

Новые идеи присылайте через [GitHub Issues](https://github.com/ckorikov/python-bar-review/issues)

## Установка

Используйте `pip` для установки зависимостей
```shell
pip install -r requirements.txt
```

затем запустите Jupyter Lab.

```shell
jupyter lab
```

Альтернативный вариант — использовать [docker](https://www.docker.com).
Для этого из подкаталога *docker* надо вызвать следующую команду.

```shell
docker-compose up
```

## Экспорт

Для экспорта ноутбуков полезна команда
```shell
jupyter nbconvert notebook.ipynb --to html --output notebook.html
```

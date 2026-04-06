# Модели с переменной волатильностью

## Источники (базы) данных

* [`FRED`](https://fred.stlouisfed.org)
* [`Yahoo Finance`](https://finance.yahoo.com)

## Необходимые библиотеки Python

|Библиотека|Описание|
|-|-|
|[`pandas`](https://pandas.pydata.org)|Табличные данные|
|[`numpy`](https://numpy.org)|Работа с массивами данных, преобразование данных|
|[`yfinance`](https://github.com/ranaroussi/yfinance)|Загрузка данных с `finance.yahoo.com`|
|[`pandas-datareader`](https://pandas-datareader.readthedocs.io/en/latest/)|Загрузка данных из внешних БД (`FRED`, `finance.yahoo.com` etc)|
|[`arch`](https://arch.readthedocs.io/en/latest/index.html)|Тесты и модели временных рядов|
|[`sktime`](https://www.sktime.net/en/stable/index.html)|Фреймворк для анализ временных рядов|
|[`scipy.stats`](https://docs.scipy.org/doc/scipy/reference/stats.html)|Статистические методы (распределения и проч)|

## Установка библиотек Python

В командной строке (Anaconda PowerShell Prompt в Windows, Terminal в MacOS) выполнить следующие команды (в дополнении в основным библиотекам)

- `pip install arch sktime`

В Google Colab недостающие библиотеки можно установить командой в первой ячейке (это нужно делать при каждом открытии ноутбука)

`%%capture --no-display`

`!pip install sktime arch`
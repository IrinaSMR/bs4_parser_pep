# Проект парсинга pep

***
### _Парсинг документов PEP_

Парсер собирает данные обо всех PEP документах, сравнивает статусы и записывает их в файл, также реализованы сбор информации о статусе версий, скачивание архива с документацией и сбор ссылок о новостях в Python.

### _Технологии проекта_

- Python 3.7
- BeautifulSoup4 - библиотека для парсинга
- Prettytable - библиотека для отображения табличных данных

### _Как запустить проект:_

Клонировать репозиторий и перейти в него в командной строке:
```
git clone https://github.com/IrinaSMR/bs4_parser_pep.git
cd bs4_parser_pep
```
Cоздать и активировать виртуальное окружение:
```
python3 -m venv env
source env/bin/activate
```
Установить зависимости из файла requirements.txt:
```
python3 -m pip install --upgrade pip
pip install -r requirements.txt
```

### _Примеры команд_

Создает файл .csv с таблицей из двух колонок: "Статус" и "Количество":
```
python main.py pep -o file
```
Выводит таблицу prettytable с тремя колонками: "Ссылка на документацию", "Версия", "Статус":
```
python main.py latest-versions -o pretty
```
Выводит ссылки на нововведения в python:
```
python main.py whats-new
```
Скачивает архив с документацией Python:
```
python main.py download
```

Автор: IrinaSMR

# Пульт охраны банка
Позволяет контролировать время нахождения сотрудников в хранилище банка. Также показывает текущие активные карты сотрудников и позволяет посмотреть историю посещений хранилища каждого сотрудника.
## Как установить
Вам потребуется настроить доступ к `БД`, создав файл `.env` и записав в нём настройки `базы данных` с которой предстоит работать.

Настройки вида:
```
DB_ENGINE=
DB_HOST=
DB_PORT=
DB_NAME=
DB_USER=
DB_PASSWORD=
```
Также в `.env` передать следующие параметры приложения:
```
APP_SECRET_KEY=
APP_DEBUG=
APP_ALLOWED_HOSTS=
```
Параметр `APP_ALLOWED_HOSTS` включает список хостов/доменов, с которыми может работать данный сайт.

Для запуска потребуется Python3. Установите необходимые сторонние библиотеки:
```
pip install -r requirements.txt
```
Запускаем проект командой:
```
python manage.py runserver
```
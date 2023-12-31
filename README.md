# Пульт охраны банка

Это сайт, который показывает охраннику все активные карты доступа. Также сайт показывает, кто находитя в хранилище и все визиты человека.

### Как установить

Для того, чтобы подключиться к базе данных нужно создать файл `.env` и в него добавить все нужные ключи.
Можно указать параметр `DEBUG`, который отвечает за полноту отображение ошибок на сайте. Также можно указать параметр `ALLOWED_HOSTS`, в котором нужно было указать домен, на котором был развёрнут сайт. Вот пример, как должен выглядеть файл:
```
SECRET_KEY=ключ шифрования вашей БД
DB_ENGINE=серверная часть БД
DB_HOST=хост вашей БД
DB_PORT=порт вашей БД
DB_NAME=имя вашей БД
DB_USER=имя пользователя, используемое при подключении к БД
DB_PASSWORD=пароль вашей БД
DEBUG=True или False для включения/ отключения дебаг-режима
ALLOWED_HOSTS=список имен хостов, которые может обслуживать этот сайт
```

Python3 должен быть уже установлен. 
Затем используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:
```powershell
pip install -r requirements.txt
```

### Как запустить

Чтобы запустить сайт, нужно ввести команду:
```powershell
python manage.py runserver
```
Далее переходим на адрес локальный адрес нашего ПК: `http://127.0.0.1:8000/`. Там и будет наш пульт охраны.

### Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).

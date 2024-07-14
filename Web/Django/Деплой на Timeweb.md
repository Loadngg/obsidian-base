1. Создать сайт и привязать домен
2. Подключиться по ssh
3. ```bash
wget https://bootstrap.pypa.io/virtualenv/3.6/virtualenv.pyz
python3 virtualenv.pyz venv
. venv/bin/activate
4. Установить зависимости
5. Перейти в папку `public_html`
6. Создать файл `.htaccess`
7. Вставить в него этот текст
8. ```
Options +ExecCGI
AddDefaultCharset utf-8
AddHandler wsgi-script .py
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^(.*)$ DjangoMySite/DjangoMySite/wsgi.py/$1 [QSA,L]
9. Создать папку с сайтом
10. Скопировать в эту папку всё содержимое проекта
11. Переписать wsgi.py
12. Переписать media и static root пути
13. Сделать миграции
14. Собрать статику
15. Создать админа
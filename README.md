# flask_todo

##Установка

git clone https://github.com/4nndr01d/flask_todo.git

cd ~/flask_todo/ && virtualenv env && source ./env/bin/activate &&
   pip install Flask && pip install Flask-SQLAlchemy && pip install PyMySQL

mysql -u root -p flask_todo < db.sql

systemctl enable /root/flask_todo/todo.service

systemctl start todo

Указать авторизационные данные для mariadb в файле config.py

------------

# О Приложении

Данное CRUD приложение является реализацией тестового задания, это todo list написанный на flask и запускаемое как демон процесс черезе systemctl, который может
Добавлять, Удалять и Редактировать записи в таблице ,которые хранятся в mariadb
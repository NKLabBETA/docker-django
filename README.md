# docker-django
ホームページ用？

#プロジェクト作成
sudo docker-compose run web django-admin.py startproject mysite .

#とりあえず
http://localhost:8000

#migration
docker exec -it docker-django_web_1 bash
python manage.py migrate

##migrationsfile作成
python manage.py makemigrations polls

##sql表示
python manage.py sqlmigrate polls 0001

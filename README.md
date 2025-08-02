# base-python-api

## Base Python API project

sudo docker build .
sudo docker compose build

## Linting
sudo docker compose run --rm app sh -c "flake8"

## Testing
sudo docker compose run --rm app sh -c "python manage.py test"

## Create new project
sudo docker compose run --rm app sh -c "django-admin startproject app ."

## Run Django App
sudo docker compose up

## Set up migrations
sudo docker compose run --rm app sh -c "python manage.py makemigrations"

## Run migration
sudo docker compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"

## Create a superuser using cli
sudo docker compose run --rm app sh -c "python manage.py createsuperuser"
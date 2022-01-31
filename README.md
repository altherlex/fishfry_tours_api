RESTful API for [fishfry_tours_app](https://github.com/altherlex/fishfry_tours_app)

[![CircleCI](https://circleci.com/gh/altherlex/fishfry_tours_api/tree/master.svg?style=svg)](https://circleci.com/gh/altherlex/fishfry_tours_api/tree/master)
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://fishfrytoursapi.herokuapp.com/api/)

Demo: https://fishfrytoursapi.herokuapp.com/api/

### Open Source Tools Used

- Django REST framework for a powerful API
- Django ORM for interacting with the database
- Bootstrapped with KnBoard
- Rest_framework
- Allauth
- Dj_rest_auth
- PostgreSQL
- Unit tests with Pytest

### Django

Have Python 3.8 installed and in PATH.
Installing Python: https://realpython.com/installing-python/

```sh
python3 --version
# Python 3.8.2
```

### Commands
```sh
virtualenv -p python3 venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip3 install -r requirements.txt

psql
CREATE DATABASE fryfish;

python manage.py migrate
python manage.py createsuperuser --username admin --email admin@admin.com
python manage.py loaddata avatars
python manage.py runserver

python manage.py loaddata db.json

# heroku
heroku run python manage.py migrate --settings=config.settings.production 
heroku run python manage.py collectstatic --no-input 
heroku run python manage.py loaddata avatars
heroku run python manage.py loaddata initial_db.json

#tests
python -m pytest
```
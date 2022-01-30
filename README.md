API for [fishfry_tours_app](https://github.com/altherlex/fishfry_tours_app)

### Open Source Tools Used

- Django REST framework for a powerful API
- Django ORM for interacting with the database
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
pip3 install -r requirements/base.txt

psql
CREATE DATABASE fryfish;

python manage.py migrate
python manage.py createsuperuser --username admin --email admin@admin.com
python manage.py loaddata avatars
python manage.py runserver

python manage.py loaddata db.json
```
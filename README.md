# Bitly Clone

This project is developed using Django and include a basic functionality of saving input data within forms and styling it using `django-crispy-forms`

## Project Setup

1. Create a new Python environment

```shell
python -m venv env
```

2. Activate Python environment

```shell
source env/Scripts/activate
```

3. Install Django

```shell
pip install django
pip install django-crispy-forms
pip install crispy-tailwind
```

1. Create the project (skip this if cloning from git, only run the first time setting up the project)

```shell
django-admin startproject config .
```

5. Run the server

```shell
python manage.py runserver
```

## Project Development Steps

1. Create app and models

```shell
python manage.py startapp links
```

2. Add app `links` by editing `INSTALLED_APPS` in `config/settings.py`

3. Create model by editing `/links/models.py`

4. Migrate the model to database

```shell
python manage.py makemigrations
python manage.py migrate
```

5. Register a new admin user by editing `/links/admin.py`

6. Create a admin user

```shell
python manage.py createsuperuser
```

7. Add data using admin page `http://127.0.0.1:8000/admin`

8. Create `/links/templates/links/index.html`

9. Set url by creating `/links/urls.py` and editing `/config/urls.py` and `/links/views.py`

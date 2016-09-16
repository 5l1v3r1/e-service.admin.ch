How to install?
===============

```
$ psql -c 'CREATE DATABASE "e_service_admin_ch"' -d postgres
$ mkdir e-service.admin.ch
$ cd e-service.admin.ch
$ git clone --recursive git@github.com:mahendrakalkura/e-service.admin.ch.git .
$ cp settings.py.sample settings.py
$ mkvirtualenv e-service.admin.ch
$ pip install -r requirements.txt
$ deactivate
```

How to run?
===========

```
$ cd e-service.admin.ch
$ workon e-service.admin.ch
$ python manage.py bootstrap
$ python manage.py insert
$ python manage.py update
$ python manage.py cities
$ python manage.py details
$ python manage.py workers
$ RESWEB_SETTINGS='.../settings.py' resweb
$ deactivate
```

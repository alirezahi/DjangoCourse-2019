# VirtualEnv

To install virtual environment:

https://virtualenvwrapper.readthedocs.io/en/latest/


# Django commands

django-admin startproject <project_name> # make intial structure of django project

python manage.py runserver # run the server
python manage.py migrate # migrate the server
python manage.py startapp <app_name> # create app folder
python manage.py createsuperuser # to make a staff user
python manage.py shell # access the shell of project



# PDB

import pdb;pdb.set_trace() # for debugging

# VSCODE PLUGINS

Django Snippet
Django Template


# Django structure
[projectname]/

├── [projectname]/

│   ├── __init__.py

│   ├── settings.py

│   ├── urls.py

│   └── wsgi.py

└── manage.py


---

# Django Model

Query:
```
Book.objects.all()
Book.objects.first()
Book.objects.last()
```

To get the sql command of query:
```
b = Book.objects.all()
qs = str(b.query)
```

To Create Django Model:

First:
```
b = Book(name='شازده کوچولو',price='30000',rate=5.5,legal=True)
b.save()
```

```
b = Book.objects.create(name='شازده کوچولو',price='30000',rate=5.5,legal=True)
or
b , is_created = Book.objects.get_or_create(name='شازده کوچولو',price='30000',rate=5.5,legal=True)
```

To delete objects:
```
Book.objects.all().delete()
```

```
Containing string:
Book.objects.filter(name__contains="sound")
Book.objects.filter(name__icontains="sound") # case-insensitive
```

```
Starting and Ending of string:
Book.objects.filter(name__startswith="sound")
Book.objects.filter(name__endswith="sound")
```

Managing Command:
```
.filter()
.exclude()
.order_by()
```


Count
```
Book.objects.all().count()
```

Admin Django Customize:
https://docs.djangoproject.com/en/2.2/ref/contrib/admin/

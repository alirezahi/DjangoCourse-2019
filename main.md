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
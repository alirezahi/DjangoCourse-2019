For example download bootstrap:

https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css

Add Static Dir to `settings.py`

~~~python3
STATICFILES_DIRS = [
    os.path.join(BASE_DIR, "static"),
    '/var/www/static/',
]
~~~

Add your static file to html:

~~~
{% load static %}
<link rel="stylesheet" href="{% static "static/boostrap.min.css %}">
~~~

1.Add template directory to settings.py
~~~python3
TEMPLATES = [
    {
        'BACKEND': 'django.template.backends.django.DjangoTemplates',
        'DIRS': ['directories-of-your-templates(html)'], # add it here
        'APP_DIRS': True,
        'OPTIONS': {
            'context_processors': [
                'django.template.context_processors.debug',
                'django.template.context_processors.request',
                'django.contrib.auth.context_processors.auth',
                'django.contrib.messages.context_processors.messages',
            ],
        },
    },
]
~~~

2.Make your html file:
```
cd templates
touch index.html
```

3.Make a `view` to return html page:
~~~python3
def main_page(request):
    return render(request, 'index.html')
~~~

4.Connect `view` to urls:
~~~python3
import main_page
urlpatterns = [
    path('hello',main_page),
]
~~~

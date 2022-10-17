# Django

## Useful Links  

## Setup
**Create Project**  
`django-admin startproject name-of-project`  

**Run server**  
`python manage.py runserver`  

## Useful Commands  
**Create App**  
`python manage.py startapp name-of-app`  

**UrlPatterns**  
```
from App import views as app_views
urlpatterns = [
    path('admin/', admin.site.urls),
    path('', app.view_name, name='name'),
]
```

## Code Snippets  

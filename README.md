# Django-REST-Framework
The popular and widely used industry-standard data interchange formats, REST API. It is the most used technique for data exchange. We will explain how to create REST APIs in Python using Django. Before diving deep into this topic, let's understand the concept of REST and how it is different from the conventional formats. Understanding REST will help to get into it in a better way. Let's have a brief introduction to the REST API.

- Basic Django Reference
- Project Setup
- Create a JSON Response with Django

<br>![Python](https://img.shields.io/badge/Python%20-%2314354C.svg?style=for-the-badge&logo=python&logoColor=white)

### Built With
![Python](https://img.shields.io/badge/Python%20-%2314354C.svg?style=for-the-badge&logo=python&logoColor=white)
[![Build Status](https://img.shields.io/travis/com/jacebrowning/template-python.svg)](https://app.travis-ci.com/github/jacebrowning/template-python)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![DjangoREST](https://img.shields.io/badge/DJANGO-REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=gray)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)![Github Pages](https://img.shields.io/badge/GitHub%20Pages-%23327FC7.svg?style=for-the-badge&logo=github&logoColor=white)
![Github Pages](https://img.shields.io/badge/GitHub%20Pages-%23327FC7.svg?style=for-the-badge&logo=github&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)

#### Running this project
### Basic Django Reference

* This is a sample for Django and Rest API Project .
To get this project up and running you should start by having Python installed on your computer. It's advised you create a virtual environment to store your projects dependencies separately. You can install virtualenv with
If you are instead looking for a [Python application](https://caremad.io/posts/2013/07/setup-vs-requirement/) template, check out one of the sibling projects:

* [jacebrowning/template-django](https://github.com/jacebrowning/template-django)

## Examples

Here are a few sample projects based on this template:

* [jacebrowning/minilog](https://github.com/jacebrowning/minilog)
* [theovoss/Chess](https://github.com/theovoss/Chess)
* [sprout42/StarStruct](https://github.com/sprout42/StarStruct)
* [MichiganLabs/flask-gcm](https://github.com/MichiganLabs/flask-gcm)
* [flask-restful/flask-restful](https://github.com/flask-restful/flask-restful)


#### Step 1- Create a virtual environment
```
pip install virtualenv
```

In Django, virtualenv is a tool used to create an isolated Python environment for a project. It allows developers to create a self-contained environment that does not interfere with other Python installations on the system.
 
```
virtualenv venv
```

That will create a new folder `env` in your project directory. Next activate it with this command on mac/linux:

```
source venv/bin/active
```
#### Step 1- Install the Library
```
pip install Django
```
#### Step 1- Create Django Project
```
django-admin createproject '<Name>'
```
Django is a popular web framework for building web applications using the Python programming language. It provides a collection of tools and libraries that make it easier to develop web applications by handling many of the low-level details of web development, such as URL routing, database connectivity, and user authentication. Django follows a "batteries included" philosophy, which means that it comes with many built-in features that are commonly used in web development, so you don't have to reinvent the wheel every time you start a new project. In summary, Django is a powerful and efficient tool for building web applications quickly and easily.


#### Step 1- Create Django application
```
$ python manage.py startapp <Name>
```
Then install the project dependencies with

```
pip install -r requirements.txt
```

Apply migrations and create your database
```
python manage.py migrate
```
Create a user with manage.py
```
python manage.py createsuperuser
```

Now you can run the project with this command

```
python manage.py runserver
```
### Step 2- What API
API is Application Programing Interface. 
* API is Middle Man eg: Real Type Example{
  Project A(Fronded)->-API-<-Project B(Backend)
  (examples:Project A is Client ,API is waiter 
  Project B is Server API is Kitchen)
  Client say to waiter bring soop And Waiter Go to Kitchen and Bring back to Client


}
### Step 2.1- What Types of API
Private 
Partner
Public
#### Prvate API
-With in Organization 
* Django Rest Framework is Our Backend and sql we Can connect to  the difrent frontend application 
Here Backend is Same but Frontend is different (Deckstop,IOS,Android,...)
-API Connection of backend to different frontend application with the help of JSON and XML
* Cuntly We using JSON
#### Partner API
-Business
eg: Prime video  <> MVD only for business
uber <> GoogleMap

#### Public API
- 3rd-parts Developer 
* Open Whether we can use 

### JSON

* Backend -> Response Form JSON
* Frontend -> Request Form JSON
- Client given Request  to Backend serch give the response to client 

 -JSON is Common Language to use for request and response

### Basics Of URL
slash with url
common url is base url
### Rest API
Rest API is Architecture.
-End Point
-Method
-Header
-Data or Body

#### End Point
url end adress 

#### Request HTTP Method

#### CRUD is 
-Create > POST request
- Read > GET request
- Update > PUT / PATCH request
- Delete > DELETE request

*Understanding URL
- https://www.imdb.com/title/tt15354916/ - individual
intivitual - GET, PUT, PATCH,DELETE

 - https://www.imdb.com/title/ - list 
GET POST

#### Headers
Status Code

#### Data
using JSON/XML

# API + REST Architecture -------------> REST API 




<br>

## Create Manual JSON

### Models.py
```py
# Create your models here.

class Movie(models.Model):
    name = models.CharField(max_length=223)
    description = models.TextField(max_length=225)
    is_active = models.BooleanField(default=True)
    
    def __str__(self) -> str:
        return self.name
```
### View.py
```bash
from django.shortcuts import render
from .models import *
from django.http import JsonResponse

def movie_list(request):
    movie = Movie.objects.all()
    data = {
        'movies' :list(movie.values())
        }
    return JsonResponse(data)

def movie_detail(request, pk):
    movie_detail = Movie.objects.get(pk=pk)
    data ={
        'name' : movie_detail.name,
        'description' : movie_detail.description ,
        'is_active' : movie_detail.is_active
    }
    return JsonResponse (data)    
```

### urls.py

### Serialization
* Model Objects (serializer) ----------->Python Dictionary ---------> JSON Data(Rendering data)
### DeSerialization(user)
* JSON Data ------------->python Dictionary --------->(deserializer) Complex Datatype

Type of Serialzers
1. serializers.serializer
2. serializers.Modelserializer
 Types of views
 1. class based views
 2. function base views
 
 Working With API
 1. Browser
 2. Postman



Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.


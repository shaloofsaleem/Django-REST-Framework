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
    - Installing dependencies with `poetry`
    - Automatic formatting with `isort` and `black`
    - Static analysis with `pylint`
    - Type checking with `mypy`
    - Docstring styling with `pydocstyle`
    - Running tests with `pytest`
    - Building documentation with `mkdocs`
    - Publishing to PyPI using `poetry`
* Tooling to launch an IPython session with automatic reloading enabled

If you are instead looking for a [Python application](https://caremad.io/posts/2013/07/setup-vs-requirement/) template, check out one of the sibling projects:

* [jacebrowning/template-django](https://github.com/jacebrowning/template-django)
* [jacebrowning/template-flask](https://github.com/jacebrowning/template-flask)

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

## Usage

Install `cookiecutter` and generate a project:

```
$ pip install cookiecutter
$ cookiecutter gh:jacebrowning/template-python -f
```

Cookiecutter will ask you for some basic info (your name, project name, python package name, etc.) and generate a base Python project for you.
Once created, run the code formatter to updates files based on your chosen names:

```
$ cd <github_repo>
$ make format
```

Finally, commit all files generated by this template.

## Updates

Run the update tool, which is generated inside each project:

```
$ bin/update
```

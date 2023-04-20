
# Django-REST-Framework

The popular and widely used industry-standard data interchange formats, REST API. It is the most used technique for data exchange. We will explain how to create REST APIs in Python using Django. Before diving deep into this topic, let's understand the concept of REST and how it is different from the conventional formats. Understanding REST will help to get into it in a better way. Let's have a brief introduction to the REST API.

See also 
- Basic Django Reference
- Project Setup
- Create a JSON Response with Django

<br>

### Built With
![Python](https://img.shields.io/badge/Python%20-%2314354C.svg?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![DjangoREST](https://img.shields.io/badge/DJANGO-REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=gray)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
### Running this project

> **DO NOT FORK** this is meant to be used from **[Use this template](https://github.com/rochacbruno/python-project-template/generate)** feature.

1. Click on **[Use this template](https://github.com/rochacbruno/python-project-template/generate)**
3. Give a name to your project  
   (e.g. `my_awesome_project` recommendation is to use all lowercase and underscores separation for repo names.)
3. Wait until the first run of CI finishes  
   (Github Actions will process the template and commit to your new repo)
4. If you want [codecov](https://about.codecov.io/sign-up/) Reports and Automatic Release to [PyPI](https://pypi.org)  
  On the new repository `settings->secrets` add your `PYPI_API_TOKEN` and `CODECOV_TOKEN` (get the tokens on respective websites)
4. Read the file [CONTRIBUTING.md](CONTRIBUTING.md)
5. Then clone your new project and happy coding!

> **NOTE**: **WAIT** until first CI run on github actions before cloning your new project.

### Basic Django Reference

- This is a sample for Django and Rest API Project .
To get this project up and running you should start by having Python installed on your computer. It's advised you create a virtual environment to store your projects dependencies separately. You can install virtualenv with

# Step 1- Create a virtual environment

[![codecov](https://codecov.io/gh/author_name/project_urlname/branch/main/graph/badge.svg?token=project_urlname_token_here)](https://codecov.io/gh/author_name/project_urlname)
[![CI](https://github.com/author_name/project_urlname/actions/workflows/main.yml/badge.svg)](https://github.com/author_name/project_urlname/actions/workflows/main.yml)

project_description

## Install it from PyPI

```bash
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
django-adm
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
```
```
API is Application Programing Interface. 
* API is Middle Man eg: Real Type Example
   -{
  Project A(Fronded)->-API-<-Project B(Backend)
  (examples:Project A is Client ,API is waiter 
  Project B is Server API is Kitchen)
  -Client say to waiter bring soop And Waiter Go to Kitchen and Bring back to Client


}
### Step 2.1- What Types of API
*Private 
*Partner
*Public
#### Prvate API
With in Organization 
Django Rest Framework is Our Backend and sql we Can connect to  the difrent frontend application 
Here Backend is Same but Frontend is different (Deckstop,IOS,Android,...)
API Connection of backend to different frontend application with the help of JSON and XML
Cuntly We using JSON
#### Partner API
Business
eg: Prime video  <> MVD only for business
uber <> GoogleMap

#### Public API
 parts Developer 
Open Whether we can use 

### JSON

Backend -> Response Form JSON
Frontend -> Request Form JSON
 Client given Request  to Backend serch give the response to client 

 JSON is Common Language to use for request and response

### Basics Of URL
slash with url
common url is base url
### Rest API
Rest API is Architecture.
End Point
Method
Header
Data or Body

#### End Point
url end adress 

#### Request HTTP Method

CRUD 
-Create > POST request
- Read > GET request
- Update > PUT / PATCH request
- Delete > DELETE request

Understanding URL
https://www.imdb.com/title/tt15354916/ - individual
intivitual - GET, PUT, PATCH,DELETE

https://www.imdb.com/title/ - list 
GET POST

#### Headers
Status Code

#### Data
using JSON/XML

API + REST Architecture -------------> REST API 




<br>
in createproject '<Name>'
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
```
```
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
With in Organization 
Django Rest Framework is Our Backend and sql we Can connect to  the difrent frontend application 
Here Backend is Same but Frontend is different (Deckstop,IOS,Android,...)
API Connection of backend to different frontend application with the help of JSON and XML
Cuntly We using JSON
#### Partner API
Business
eg: Prime video  <> MVD only for business
uber <> GoogleMap

#### Public API
 parts Developer 
Open Whether we can use 

### JSON

Backend -> Response Form JSON
Frontend -> Request Form JSON
 Client given Request  to Backend serch give the response to client 

 JSON is Common Language to use for request and response

### Basics Of URL
slash with url
common url is base url
### Rest API
Rest API is Architecture.
End Point
Method
Header
Data or Body

#### End Point
url end adress 

#### Request HTTP Method

CRUD is -Create > POST request
- Read > GET request
- Update > PUT / PATCH request
- Delete > DELETE request

Understanding URL
https://www.imdb.com/title/tt15354916/ - individual
intivitual - GET, PUT, PATCH,DELETE

https://www.imdb.com/title/ - list 
GET POST

#### Headers
Status Code

#### Data
using JSON/XML

API + REST Architecture -------------> REST API 




<br>

## Usage

```py
from project_name import BaseClass
from project_name import base_function

BaseClass().base_method()
base_function()
```

```bash
$ python -m project_name
#or
$ project_name
```

## Development

Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.

  **or Run `make init` after cloning to generate a new project based on a template.**
- 📦 A basic [setup.py](setup.py) file to provide installation, packaging and distribution for your project.  
  Template uses setuptools because it's the de-facto standard for Python packages, you can run `make switch-to-poetry` later if you want.
- 🤖 A [Makefile](Makefile) with the most useful commands to install, test, lint, format and release your project.
- 📃 Documentation structure using [mkdocs](http://www.mkdocs.org)
- 💬 Auto generation of change log using **gitchangelog** to keep a HISTORY.md file automatically based on your commit history on every release.
- 🐋 A simple [Containerfile](Containerfile) to build a container image for your project.  
  `Containerfile` is a more open standard for building container images than Dockerfile, you can use buildah or docker with this file.
- 🧪 Testing structure using [pytest](https://docs.pytest.org/en/latest/)
- ✅ Code linting using [flake8](https://flake8.pycqa.org/en/latest/)
- 📊 Code coverage reports using [codecov](https://about.codecov.io/sign-up/)
- 🛳️ Automatic release to [PyPI](https://pypi.org) using [twine](https://twine.readthedocs.io/en/latest/) and github actions.
- 🎯 Entry points to execute your program using `python -m <project_name>` or `$ project_name` with basic CLI argument parsing.
- 🔄 Continuous integration using [Github Actions](.github/workflows/) with jobs to lint, test and release your project on Linux, Mac and Windows environments.

> Curious about architectural decisions on this template? read [ABOUT_THIS_TEMPLATE.md](ABOUT_THIS_TEMPLATE.md)  
> If you want to contribute to this template please open an [issue](https://github.com/rochacbruno/python-project-template/issues) or fork and send a PULL REQUEST.

[❤️ Sponsor this project](https://github.com/sponsors/rochacbruno/)

<!--  DELETE THE LINES ABOVE THIS AND WRITE YOUR PROJECT README BELOW -->

---
# project_name

[![codecov](https://codecov.io/gh/author_name/project_urlname/branch/main/graph/badge.svg?token=project_urlname_token_here)](https://codecov.io/gh/author_name/project_urlname)
[![CI](https://github.com/author_name/project_urlname/actions/workflows/main.yml/badge.svg)](https://github.com/author_name/project_urlname/actions/workflows/main.yml)

project_description

## Install it from PyPI

```bash
pip install project_name
```

## Usage

```py
from project_name import BaseClass
from project_name import base_function

BaseClass().base_method()
base_function()
```

```bash
$ python -m project_name
#or
$ project_name
```

## Development

Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.

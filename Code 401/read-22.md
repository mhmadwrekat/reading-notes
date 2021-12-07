# Django Custom User

---
## Django Best Practices: Custom User Model

Django ships with a built-in User model for authentication and if you'd like a basic tutorial on how to implement log in, log out, sign up and so on see the Django Login and Logout tutorial for more .

However, for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects .

But how to implement one? The official documentation example is not actually what many Django experts recommend using. There is a far easier yet still powerful approach to starting off new Django projects with a custom user model .

A process flowchart of how Django handles form requests is shown below, starting with a request for a page containing a form (shown in green) .


![Django Custom User](https://miro.medium.com/max/1200/1*uaNY18SZjv5OUCIwqr3WPg.png)

---
## AbstractUser vs AbstractBaseUser

There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. Seriously, don't mess with it unless you really know what you're doing. And if you did, you wouldn't be reading this tutorial, would you ?

So we'll use AbstractUser which actually subclasses AbstractBaseUser but provides more default configuration . 

---
## Superuser

It's helpful to create a superuser that we can use to log in to the admin and test out log in/log out. On the command line type the following command and go through the prompts.

    (accounts) $ python manage.py createsuperuser

---
## Templates / Views / URLs

Our goal is a homepage with links to log in, log out, and sign up. Start by updating settings.py to use a project-level templates directory.

```
# config/settings.py
TEMPLATES = [
    {
        ...
        'DIRS': [str(BASE_DIR.joinpath('templates'))], # new
        ...
    },
]
```
Then set the redirect links for log in and log out, which will both go to our home template. Add these two lines at the bottom of the file .

```
# config/settings.py
LOGIN_REDIRECT_URL = 'home'
LOGOUT_REDIRECT_URL = 'home'
```

Create a new project-level templates folder and within it a registration folder as that's where Django will look for the log in template. We will also put our signup.html template in there .

```
(accounts) $ mkdir templates
(accounts) $ mkdir templates/registration
```

Then create four templates:

```
(accounts) $ touch templates/registration/login.html
(accounts) $ touch templates/registration/signup.html
(accounts) $ touch templates/base.html
(accounts) $ touch templates/home.html
```
---
## Django X

***Installation***

DjangoX can be installed via Pip, Pipenv, or Docker depending upon your setup. To start, clone the repo to your local computer and change into the proper directory .

    $ git clone https://github.com/wsvincent/djangox.git
    $ cd djangox

***Pip***

    $ python3 -m venv djangox
    $ source djangox/bin/activate
    (djangox) $ pip install -r requirements.txt
    (djangox) $ python manage.py migrate
    (djangox) $ python manage.py createsuperuser
    (djangox) $ python manage.py runserver
    # Load the site at http://127.0.0.1:8000

![Django X](https://github.com/wsvincent/djangox/raw/master/homepage.png)

***Pipenv***

    $ pipenv install
    $ pipenv shell
    (djangox) $ python manage.py migrate
    (djangox) $ python manage.py createsuperuser
    (djangox) $ python manage.py runserver
    # Load the site at http://127.0.0.1:8000

***Docker***

    $ docker build .
    $ docker-compose up -d
    $ docker-compose exec web python manage.py migrate
    $ docker-compose exec web python manage.py createsuperuser
    # Load the site at http://127.0.0.1:8000

> ***For Docker, the INTERNAL_IPS configuration in config/settings.py must be updated to the following :***

    # config/settings.py
    # django-debug-toolbar  
    import socket
    hostname, _, ips = socket.gethostbyname_ex(socket.gethostname())
    INTERNAL_IPS = [ip[:-1] + "1" for ip in ips]

***Setup***

    # Run Migrations
    (djangox) $ python manage.py migrate

    # Create a Superuser
    (djangox) $ python manage.py createsuperuser

    # Confirm everything is working:    
    (djangox) $ python manage.py runserver

    # Load the site at http://127.0.0.1:8000

---
## Sources and references

- ***[Django Custum User Model .](https://learndjango.com/tutorials/django-custom-user-model)***

- ***[DjangoX .](https://github.com/wsvincent/djangox)***

- ***[Creating a Custom User Moel .](https://www.youtube.com/watch?v=eCeRC7E8Z7Y&t=59s)***

- ***[Abstract User, User Profile and Signals in Django .](https://www.youtube.com/watch?v=EudKs1HPUfE)***

- ***[Substituting a custom User model .](https://docs.djangoproject.com/en/3.0/topics/auth/customizing/#auth-custom-user)***
---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

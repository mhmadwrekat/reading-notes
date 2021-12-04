# Intro to Django

***Creating a project***

If this is your first time using Django, you’ll have to take care of some initial setup. Namely,
you’ll need to auto-generate some code that establishes a Django project – a collection of settings for an instance of Django, 
including database configuration, Django-specific options and application-specific settings.

*From the command line, cd into a directory where you’d like to store your code and Write this in the command line :*

>  django-admin startproject mysite


***You will see These files :***

- The outer mysite/ root directory is a container for your project. Its name doesn’t matter to Django; you can rename it to anything you like.
- manage.py: A command-line utility that lets you interact with this Django project in various ways. You can read all the details about manage.py in django-admin and manage.py.
- The inner mysite/ directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).
- mysite/init.py: An empty file that tells Python that this directory should be considered a Python package. If you’re a Python beginner, read more about packages in the official Python docs.
- mysite/settings.py: Settings/configuration for this Django project. Django settings will tell you all about how settings work.
- mysite/urls.py: The URL declarations for this Django project; a “table of contents” of your Django-powered site. You can read more about URLs in URL dispatcher.
- mysite/asgi.py: An entry-point for ASGI-compatible web servers to serve your project. See How to deploy with ASGI for more details.
- mysite/wsgi.py: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.

## The development server

*Let’s verify your Django project works. Change into the outer mysite directory, if you haven’t already, and run the following commands :*

> python manage.py runserver

You’ve started the Django development server, a lightweight Web server written purely in Python. We’ve included this with Django so you can develop things rapidly, 
without having to deal with configuring a production server – such as Apache – until you’re ready for production.

## Django Software Foundation

The DSF supports and maintains Django in a number of capacities. The largest expense, by far, is the Fellows Program, paid contractors who triage tickets, manage releases,
and generally perform the unsexy but necessary work needed to keep Django on track.

Tim Graham was the inaugural fellow during its 3-month pilot in the fall of 2014 and became a full-time fellow in 2015. He remained in this role until 2018 before transitioning to a part-time role.
Carlton Gibson joined as a part-time Fellow in 2018 and in 2019 Mariusz Felisiak took over from Tim Graham.

## Technical Organization

The DSF handles legal, financial, and administrative matters for Django. 
But there is a separate organizational structure for the technical team.

Historically, Django followed Python’s model of having a Benevolent Dictator for Life, that is, a project founder who retained final say for disputes/arguments within the community. 
Adrian Holovaty and Jacob Kaplan-Moss functioned as Django’s dual-BDFLs from 2005 until their retirement in 2014.


![Django](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR3UBgazU5UU1XOY-G0WTGbnDwMCcXauelFXA&usqp=CAU)

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

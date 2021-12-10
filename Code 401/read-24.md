# Django REST Framework & Dock

---
##  Beginner’s Guide to Docker

***Docker*** 

which is a way to isolate and run entire applications. With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated: programming language, software packages, databases, and more .

With Docker we now longer have to mess around with virtual environments. We can faithfully reproduce a production environment locally. And Docker can be shared among team members so everyone is working on the same setup. Wins all around .

***Containers vs Virtual Environments***

Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great .

But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment .

Also we can’t run a production database or other services within virtual environments so compared to Docker containers they are far more limited .

---
## Install Docker

Ok, enough theory. Let’s start using Docker .

To install Docker we need to **[download the desktop app on our computer](https://www.docker.com/get-started)** and create a free account. The initial download of Docker might take some time to download. It’s a big file. Feel free to stretch your legs at this point!

Once Docker is done installing we can confirm the correct version is running. It should be at least version 19.

    $ docker --version
    Docker version 19.03.5, build 633a0ea

Docker Compose is an additional tool that is automatically included with Mac and Windows downloads of Docker. However if you are on Linux, you will need to add it manually. You can do this by running the command 
> sudo pip install docker-compose 

after your Docker installation is complete.

Now run the command below to confirm you have a working version of it, too. The version should be **at least 1.24.x .**

    $ docker-compose --version  
    docker-compose version 1.24.1, build 4667896b
---
## Django for APIs - Library Website

Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured .


***Traditional Django***

First we need a dedicated directory on our computer to store the code. This can live anywhere but for convenience, if you are on a Mac, we can place it in the Desktop folder. The location really does not matter; it just needs to be easily accessible .

***Browsable API***

With the local server still running in the first command line console, navigate to our API endpoint in the web browser at **http://127.0.0.1:8000/api/.**


Django REST Framework provides this visualization by default. And there is a lot of functionality built into this page that we will explore throughout the book. For now I want you to compare this page with the raw JSON endpoint. Click on the “GET” button and select “json” from the dropdown menu .

![Django & Docker](https://miro.medium.com/max/1040/1*2yGunnADb78nmkuSFXCriQ.png)

---
## Sources and references

- ***[Beginner’s Guide to Docker .](https://wsvincent.com/beginners-guide-to-docker/)***

- ***[Django for APIs - Library Website .](https://djangoforapis.com/library-website-and-api/)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

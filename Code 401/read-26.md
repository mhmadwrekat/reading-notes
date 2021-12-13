# Authentication & Production Server

---
## JSON Web Tokens

![JSON Web Tokens](https://www.devonblog.com/wp-content/uploads/2018/08/jwt_05.jpg)


***What is JSON Web Token ?***

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA .


***When should you use JSON Web Tokens ?***

Here are some scenarios where JSON Web Tokens are useful :

- ***Authorization :***
This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains .

- **Information Exchange :** 
JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with .


***What is the JSON Web Token structure ?***

In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are :

1. Header
2. Payload
3. Signature

---
## DRF JWT Authentication

***How JWT Works ?***

The JWT is just an authorization token that should be included in all requests :

    curl http://127.0.0.1:8000/hello/ -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNTQzODI4NDMxLCJqdGkiOiI3ZjU5OTdiNzE1MGQ0NjU3OWRjMmI0OTE2NzA5N2U3YiIsInVzZXJfaWQiOjF9.Ju70kdcaHKn1Qaz8H42zrOYk0Jx9kIckTn9Xx7vhikY'


The JWT is acquired by exchanging an username + password for an access token and an refresh token.

The access token is usually short-lived (expires in 5 min or so, can be customized though).

The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.

***Installation & Setup***

we are going to use the djangorestframework_simplejwt library, recommended by the DRF developers .

> pip install djangorestframework_simplejwt


***settings.py***
```
REST_FRAMEWORK = {
    'DEFAULT_AUTHENTICATION_CLASSES': [
        'rest_framework_simplejwt.authentication.JWTAuthentication',
    ],
}
```

***urls.py***
```
from django.urls import path
from rest_framework_simplejwt import views as jwt_views

urlpatterns = [
    # Your URLs...
    path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
    path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
]
```

---
## Django Runserver Is Not Your Production Server

A Production Stack

You want to only use tech in production, which is reliable, well tested and has been around for a while.

A production setup usually consists of multiple components, each designed and built to be really good at one specific thing. They are fast, reliable and very focused.

When a request arrives at your server, it should be passed to a dedicated web server. Nginx is an example for a good web server.

This is an application, which is great at serving static files from disk (your css and js files for example) and handling multiple requests at once. If the request is not for a static file, but should be processed by your application, the webserver is configured to pass this request to the next component.


***How Does Django Fit In ?***

Your Django app does not actually run as you would think a server would - waiting for requests and reacting to them. Your project provides a **uwsgi.py file**, which contains a function to be called by the application server. This function gets a Python object representing the incoming request .

This function calls your code, and produces a response object which is passed to the WSGI server. There the response is translated into a *HTTP* response and is passed back to the web server, which finally delivers it to the user .


***In Conclusion***

If you want to run Django in production, be sure to use a production-ready web server like Nginx, and let your app be handled by a WSGI application server like **[Gunicorn](https://vsupalov.com/what-is-gunicorn/)** .

If you plan on running on **Heroku**, a web server is provided implicitly. You don’t have to take care of it. You just need to specify a command to run your application server (again, Gunicorn is fine) in the Procfile.

---
## Sources and references

- ***[JSON Web Tokens .](https://jwt.io/introduction/)***

- ***[DRF JWT Authentication .](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)***

- ***[Django Runserver Is Not Your Production Server .](https://vsupalov.com/django-runserver-in-production/)***

- ***[JWT with DRF .](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)***

- ***[Gunicorn .](https://gunicorn.org/)***

- ***[Django Migrations Primer .](https://realpython.com/django-migrations-a-primer/)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

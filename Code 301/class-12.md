# CRUD

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Status Codes Based On REST Methods|First Paragraph|
|lovers of reading|Second Paragraph|
|Things I want to know more about|In The Last|

---
## Status Codes Based On REST Methods

* ### ***HTTP Status Codes*** 

A status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. The first digit defines the class of the status. A status code comes with a reason phrase. The code is for programmatic recognition the phrase is for humans to understand what happened .


* ### ***Status Classes*** 

![Status Classes](https://en.ryte.com/wiki/nsfr_img_auth.php/9/9d/httpStatusCode_de_en.png)

> If we understand the class a status code is in, we can locate problems more quickly .

* **100 - 199**
These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body .

* **200 - 299**
These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending .

* **300 - 399**
These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location .

* **400 - 499**
These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request .

* **500 - 599**
These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request .

* ### ***CRUD***
 
![CRUD](https://www.dorusomcutean.com/wp-content/uploads/2020/03/crud.jpg)

#### ( Create , Read , Update , Delete )

1. **CREATE :** The create action is usually implemented via HTTPs POST method. In RESTful APIs, these endpoints are used to create new resources or access tokens .

2. **READ :** The read action gets implemented via HTTPs GET method and used to fetch resource representations. Asynchronous responses aren’t much of a thing here, because the reason for asynchronous processing is often that the resource doesn’t exist yet and has to be created, so it’s a create action anyway .

3. **UPDATE :** An update can be implemented with an HTTP PUT or PATCH method. The difference lies in the amount of data the client has to send to the backend .

4. **DELETE :** The delete action can be implemented with the HTTP DELETE method .

* ### ***API Changes*** 

If our API lives long enough, sooner or later it will change its structure. It’s best practice to avoid breaking changes and the redirection class of status codes can help with this because some clients follow their Location header automatically .

---
## ***For lovers of reading*** :

<img src='https://www.lovereading.co.uk/content/images/love-reading-generic-facebook-image.jpg' height='300'>


**[More about Status Codes Based On REST Methods ......](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)**

**[More about Build A REST API With Node.js, Express, & MongoDB ......](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)**

---
## Things I want to know more about

* ### ***Diversity & Inclusion in the Tech Industry .***

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

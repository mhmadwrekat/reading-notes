# APIs

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|API Design Best Practices|First Paragraph|
|lovers of reading|Second Paragraph|
|Things I want to know more about|In The Last|

---
## API Design Best Practices

* ### ***What is REST ?*** 

![REST](https://devwithus.com/assets/images/posts/spring/api-acronym.jpg)

In 2000, Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.

* ### ***REST APIs are designed around a ____.*** 
> REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client .

* ### ***What are the most common HTTP verbs ?***

There are 4 basic HTTP verbs we use in requests to interact with resources in a REST system :

1. **GET** retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource .
2. **POST** creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources .
3. **PUT** either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated .
4. **PATCH** performs a partial update of a resource. The request body specifies the set of changes to apply to the resource .
5. **DELETE** removes the resource at the specified URI .

![HTTP verbs](https://customersdb.blob.core.windows.net/org/1006/photo/ac901bfc-d6a2-47cc-817f-b5b068c684d1.png)

* ### ***Versioning a RESTful web API*** 
    
It is highly unlikely that a web API will remain static. As business requirements change new collections of resources may be added, the relationships between resources might change, and the structure of the data in resources might be amended. While updating a web API to handle new or differing requirements is a relatively straightforward process, you must consider the effects that such changes will have on client applications consuming the web API. The issue is that although the developer designing and implementing a web API has full control over that API, the developer does not have the same degree of control over client applications, which may be built by third-party organizations operating remotely. The primary imperative is to enable existing client applications to continue functioning unchanged while allowing new client applications to take advantage of new features and resources .

* ### ***URI versioning***

Each time you modify the web API or change the schema of resources, you add a version number to the URI for each resource. The previously existing URIs should continue to operate as before, returning resources that conform to their original schema .

---
## ***For lovers of reading*** :

<img src='https://www.lovereading.co.uk/content/images/love-reading-generic-facebook-image.jpg' height='300'>


**[More about RegExr ......](https://regexr.com/)**

**[How would you match your name using RegEx ? ......](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)**

---
## Things I want to know more about

* ### ***FUNCTIONAL PROGRAMMING .***

* ### ***Node JS - Modules and require () .***

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

# In memory storage

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Understanding the JavaScript Call Stack|First Paragraph|
|JavaScript error messages|Second Paragraph|
|lovers of reading|Third Paragraph|
|Things I want to know more about|In The Last|

---
## Understanding the JavaScript Call Stack

* ### ***What is a ‘callBack’ ?*** 

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns .

* ### ***What does LIFO mean ?*** 

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns .

![LIFO](https://media.geeksforgeeks.org/wp-content/uploads/20200427215327/LIFO.png)

* ### ***What causes a stack overflow ?*** 

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point , The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error .

#### ***Example :*** 

    function callMyself(){
    callMyself();
    }
    callMyself();

The callMyself() will run until the browser throws a “Maximum call size exceeded”. And that is a stack overflow.

![example](https://cdn-media-1.freecodecamp.org/images/lvjT-ud6XfVQ5KYVWxZZWkKeVTgtJqFD0pWv)

---
## JavaScript error messages

* ### ***Types of error messages :*** 

The first thing that indicates you that something is wrong with your code is the (in)famous error message that the one we saw just moments ago, it usually appears on your console (being developer tools of the browser, terminal or whatever else you are using) .

![ERRORS](https://www.notionwizard.com/wp-content/uploads/2021/04/Error-Illustration.jpg)

*For those already used to programming, reading an error message is like second nature, for everybody else, is something you learn either you like it or not so might as well talk a bit about each of them :*


**1. Reference errors :** This is as simple as when you try to use a variable that is not yet declared you get this type os errors .

**2. Syntax errors :** I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse .

**3. Range errors :** Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up .

**4. Type errors :** Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable .

---
## ***For lovers of reading*** :

<img src='https://www.lovereading.co.uk/content/images/love-reading-generic-facebook-image.jpg' height='300'>


**[More about Understanding the JavaScript Call Stack ......](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)**

**[More about JavaScript error messages ......](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)**

---
## Things I want to know more about

* ### ***Mongo .***

* ### ***Mongoose .***

* ### ***Nosql Vs Sql .***

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

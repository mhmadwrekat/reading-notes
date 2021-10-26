# Local Storage


*The Past, Present, and Future of Local Storage for Web Applications*

> Historically , web applications have had none of these luxuries , Cookies were invented early in the web’s history , and indeed they can be used for persistent local storage of small amounts of data .

### they have three potentially dealbreaking downsides :
1. Cookies are included with every HTTP request , thereby slowing down your web application by needlessly transmitting the same data over and over .
2. Cookies are included with every HTTP request , thereby sending data unencrypted over the internet (unless your entire web application is served over SSL) .
3. Cookies are limited to about 4 KB of data — enough to slow down your application , but not enough to be terribly useful .

![HTML5](https://clementbuchanan.github.io/reading-notes/images/html5.jpg)



---
### What we really want ?
* a lot of storage space
* on the client
* that persists beyond a page refresh
*isn’t transmitted to the server

> Before **HTML5** , all attempts to achieve this were ultimately unsatisfactory in different ways .

---
### USING HTML5 STORAGE

*HTML5* Storage is based on named key/value pairs , You store data based on a named key then you can retrieve that data with the same key , The named key is a *string* , The data can be any type supported by JavaScript , including *strings* , *Booleans* , *integers* , or *floats* , However , the data is actually stored as a string , If you are storing and retrieving anything other than strings , you will need to use functions like **parseInt()** or **parseFloat()** to coerce your retrieved data into the expected JavaScript datatype .

---
**[Read more.....](http://diveinto.html5doctor.com/storage.html)**

![Shwos Pic](https://peerbits-wpengine.netdna-ssl.com/wp-content/uploads/2018/11/web-application-architecture-components.jpg)


---
##### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
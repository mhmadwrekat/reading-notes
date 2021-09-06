> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Domain Modeling|First Paragraph|
|HTML tables|second Paragraph|
|JS Functions , Methods , and Objects|Third Paragraph|
|Quiz|In The Last|

---
## Domain Modeling
what is the Domain Modeling ?

Domain modeling is the process of creating a conceptual model in code for a specific problem , A model describes the various entities , their attributes and behaviors , as well as the constraints that govern the problem domain , An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object - oriented model .

### some tips to follow when building your own domain models :
* When modeling a single entity that'll have many instances , build self-contained objects with the same attributes and behaviors .
* Model its attributes with a constructor function that defines and initializes properties .
* Model its behaviors with small methods that focus on doing one job well .
* Create instances using the new keyword followed by a call to a constructor function .
* Store the newly created object in a variable so you can access its properties and methods from outside .
* Use the this variable within methods so you can access the object's properties and methods from inside .

[Read Article](https://github.com/codefellows/domain_modeling#domain-modeling)

![problem domain](https://mozaicworks.com/wp-content/uploads/2016/10/Screen-Shot-2016-10-13-at-15.18.16.png)

---
## HTML tables
> *There are several types of information that need to be displayed in a grid or table , For example: sports results , stock reports , train timetables.*

### Basic Table Structure :
< table>

< tr>

< td>15< /td>

< td>15< /td>

< td>30< /td>

< /tr>

< tr>

< td>45< /td>

< td>60< /td>

< td>45< /td>

< /tr>

< tr>

< td>60< /td>

< td>90< /td>

< td>90< /td>

< /tr>

< /table>

![HTML table](https://res.cloudinary.com/practicaldev/image/fetch/s--Zhu5E2Bm--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/02lxssgxrwv7ywp2lhix.jpg)

---
## JS Functions , Methods , and Objects

> Objects can also have methods .

> Methods are actions that can be performed on objects .

> Methods are stored in properties as function definitions .

**Example** in Object :

var hotel = new Object();

hotel.name= 'Park';

hotel.rooms = 120;

hotel .booked = 77;

hotel .checkAvailability = function()

return this . rooms - this.booked;
} ;

var elName = document.getElementByid('hotelName');

elName.textContent = hotel . name;

var elRooms = document .getElementByid('rooms');

elRooms .textContent = hotel .checkAvailability(};


[For more detail : JS Book](https://www.goodreads.com/book/show/16219704-javascript-and-jquery)

![JS Objects](https://www.tutsmake.com/wp-content/uploads/2020/05/JavaScript-Objects.jpeg)

---
### [Take Quiz](https://mhmadwrekat.github.io/reading-notes/quizclass07)

---
##### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)


---
<b>
<p align="center">
© Mohammad alwrekat
</p>
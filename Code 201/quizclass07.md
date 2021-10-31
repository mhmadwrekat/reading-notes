## Quiz Class07

---

![Good Luck](https://images.assetsdelivery.com/compings_v2/venimo/venimo1705/venimo170500047.jpg)

---
**1.** 

what is the Domain Modeling ?

---
**2.** 

some tips to follow when building your own domain models ?

---
**3.** 

Example in Table in HTML ?

---
**4.** 

**Example** in Object ?

---
## Answers 
**1.** 

Domain modeling is the process of creating a conceptual model in code for a specific problem , A model describes the various entities , their attributes and behaviors , as well as the constraints that govern the problem domain , An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object - oriented model .

---
**2.**

* When modeling a single entity that'll have many instances , build self-contained objects with the same attributes and behaviors .
* Model its attributes with a constructor function that defines and initializes properties .
* Model its behaviors with small methods that focus on doing one job well .
* Create instances using the new keyword followed by a call to a constructor function .
* Store the newly created object in a variable so you can access its properties and methods from outside .
* Use the this variable within methods so you can access the object's properties and methods from inside .


---
**3.**

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

---
**4.** 

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

---

##### [Back](https://mhmadwrekat.github.io/reading-notes/Code 201/class07)

---
##### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
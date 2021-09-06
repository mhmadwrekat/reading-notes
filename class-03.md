# Passing Functions as Props

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|lists and keys|First Paragraph|
|The Spread Operator|second Paragraph|
|How to Pass Functions Between Components|Third Paragraph|
|lovers of reading|Forth Paragraph|
|Things I want to know more about|In The Last|

---
## lists and keys

![lists and keys](https://i.morioh.com/200626/ec9a9e94.jpg)

* ### ***Lists***

Showing a list of elements happened almost in every project I was ever writing. And React really simplifies the rendering of lists inside the JSX by supporting the Javascript **. map** method.

The **. map** method in Javascript iterates through the parent array and calls a function on every element of that array. Then it creates a new array with transformed values. It doesn’t change the parent array.

* ### ***Keys***

When creating a list of elements in a way you can see above, there’s one more necessary thing, and it’s a key.

key is a special attribute that you need to include in the element, and it should be a string. Keys in each list should be unique, which means that you shouldn’t use values that can be the same as the key. In other words, keys should be unique among the siblings, not globally.

---
## The Spread Operator

![The Spread Operator](https://i.ytimg.com/vi/pYI-UuZVtHI/maxresdefault.jpg)

* ### ***What is the spread operator ?***

InJavaScript, spread syntax refers to the use of an ellipsis of three dots **(…)** toexpand an iterable object into the list of arguments.

* ### ***Things that the spread operator can do ?***

* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array

### ***Examples :***

**1. Example of using the spread operator to combine two arrays :**

>
    const fruits = ['🍏','🍊','🍌','🍉','🍍']
    const moreFruits = [...fruits];
    console.log(moreFruits) // Array(5) [ "🍏", 
    "🍊", "🍌", "🍉", "🍍" ]
    fruits[0] = '🍑'
    console.log(...[...fruits,'...',...moreFruits]
    ) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

**2. Example of combine arrays :**
>
    [...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
    [..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

    const hello = {hello: "😋😛😜🤪😝"}
    const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

    const helloWorld = {...hello,...world}
    console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }

**3. Example of using the spread operator to combine two arrays :**
>
    const myArray = [`🤪`,`🐻`,`🎌`]
    const yourArray = [`🙂`,`🤗`,`🤩`]
    const ourArray = [...myArray,...yourArray]
    console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

**4. Example of Adding an item to a list :**
>
    const fewFruit = ['🍏','🍊','🍌']
    const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
    console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

---
## How to Pass Functions Between Components


>First, you'll need to create two components, one parent and one child.

>Next, you'll import the child component in the parent component and return it.

>Then you'll create a function and a button to trigger that function. Also, you'll create a state using the useState Hook to manage the data.

**[Watch Video .......](https://www.youtube.com/watch?v=IYvD9oBCuJI)**

---
## ***For lovers of reading*** :

<img src='https://www.lovereading.co.uk/content/images/love-reading-generic-facebook-image.jpg' height='300'>


**[React Tutorial through ‘Declaring a Winner  ......](https://reactjs.org/tutorial/tutorial.html)**


**[React Docs - Lifting State Up  ......](https://reactjs.org/docs/lifting-state-up.html)**

---
## Things I want to know more about

* React - Forms .
* The Conditional (Ternary) Operator Explained in React .

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

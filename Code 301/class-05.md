# Putting it all together

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Thinking in React|First Paragraph|
|lovers of reading|Second Paragraph|
|Things I want to know more about|In The Last|

---
## Thinking in React

> One of the many great parts of React is how it makes you think about apps as you build them .

![Thinking in React](https://image.slidesharecdn.com/5otyxvctmo17mwwg9tpe-signature-b3cb803483589fcfdfab2151355b3b43eb21fac6d43305da6c7e00f9f2e268d1-poli-170717035714/95/thinking-in-react-1-638.jpg?cb=1500263883)


* ### ***Break The UI Into A Component Hierarchy***

The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components !


* ### ***Build A Static Version in React*** 
    
To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it .


* ### **Identify The Minimal (but complete) Representation Of UI State**

To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with state .

![State](https://qph.fs.quoracdn.net/main-qimg-2533708ec99c4e983d7c4bf53e8b8284)


* ### **Identify Where Your Code Should Live**

Remember: React is all about one-way data flow down the component hierarchy. It may not be immediately clear which component should own what state. This is often the most challenging part for newcomers to understand, so follow these steps to figure it out :

1. Identify every component that renders something based on that state .

2. Find a common owner component (a single component above all the components that need the state in the hierarchy) .

3. Either the common owner or another component higher up in the hierarchy should own the state .

4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component .

* ### **Add Inverse Data Flow**

React makes this data flow explicit to help you understand how your program works, but it does require a little more typing than traditional two-way data binding .

If you try to type or check the box in the current version of the example, you’ll see that React ignores your input. This is intentional, as we’ve set the value prop of the input to always be equal to the state passed in from FilterableProductTable .

---
## ***For lovers of reading*** :

<img src='https://www.lovereading.co.uk/content/images/love-reading-generic-facebook-image.jpg' height='300'>


**[More aboutt Thinking in React  ......](https://reactjs.org/docs/thinking-in-react.html)**

---
## Things I want to know more about

* ### ***Reasons for Pair Programming .***

* ### ***NODE.JS .***

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

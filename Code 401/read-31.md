# React 2

---
## Conditional Rendering

In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

Consider these two components:

    function UserGreeting(props) {
        return <h1>Welcome back!</h1>;
    }
    function GuestGreeting(props) {
        return <h1>Please sign up.</h1>;
    }

We’ll create a Greeting component that displays either of these components depending on whether a user is logged in:

    function Greeting(props) {
        const isLoggedIn = props.isLoggedIn;
        if (isLoggedIn) {
            return <UserGreeting />;
        }
        return <GuestGreeting />;
    }
    ReactDOM.render(
      // Try changing to isLoggedIn={true}:
        <Greeting isLoggedIn={false} />,
        document.getElementById('root')
    );

Try it on CodePen

This example renders a different greeting depending on the value of isLoggedIn prop.

---
## Lists and Keys


![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)



***Basic List Component***

Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

    function NumberList(props) {
    const numbers = props.numbers;
    const listItems = numbers.map((number) =>
        <li>{number}</li>
    );
    return (
        <ul>{listItems}</ul>
    );
    }
    const numbers = [1, 2, 3, 4, 5];
    ReactDOM.render(
      <NumberList numbers={numbers} />,
      document.getElementById('root')   
    );

When you run this code, you’ll be given a warning that a key should be provided for list items. A “key” is a special string attribute you need to include when creating lists of elements. 

***Keys***

We don’t recommend using indexes for keys if the order of items may change. This can negatively impact performance and may cause issues with component state. Check out Robin Pokorny’s article for an in-depth explanation on the negative impacts of using an index as a key. If you choose not to assign an explicit key to list items then React will default to using indexes as keys .

---
## Forms

HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:

    <form>
    <label>
        Name:
        <input type="text" name="name" />
    </label>
    <input type="submit" value="Submit" />
    </form>

This form has the default HTML form behavior of browsing to a new page when the user submits the form. If you want this behavior in React, it just works. But in most cases, it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”.

---
## Composition vs Inheritance

***Containment***

Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”.


***Specialization***

Sometimes we think about components as being “special cases” of other components. For example, we might say that a WelcomeDialog is a special case of Dialog

---
## Sources and references

- ***[React - Conditional Rendering .](https://reactjs.org/docs/conditional-rendering.html)***

- ***[React - Lists & Keys .](https://reactjs.org/docs/lists-and-keys.html)***

- ***[React - Forms .](https://reactjs.org/docs/forms.html)***

- ***[React - Lifting State .](https://reactjs.org/docs/lifting-state-up.html)***

- ***[React - Composition vs Inheritance .](https://reactjs.org/docs/composition-vs-inheritance.html)***

- ***[Thinking in React .](https://reactjs.org/docs/thinking-in-react.html)***

- ***[Hero Icons .](https://www.youtube.com/watch?v=cVa1UiKPJN8)***

- ***[React - Comprehensive Guide .](https://ui.dev/reactjs-tutorial-a-comprehensive-guide-to-building-apps-with-react/)***

- ***[Heroicons .](https://heroicons.com/)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

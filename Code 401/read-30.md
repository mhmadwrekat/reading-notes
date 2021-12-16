# React 1

---
## ES6 Overview

***Variables and constant feature comparison***

I explain the concepts of scope and the differences between let, var, and const in the Understanding Variables, Scope, and Hoisting in JavaScript resource on DigitalOcean. This table provides a brief overview .

| Keyword | Scope | Hoisting | Can Be Reassigned | Can Be Redeclared |
|---------|-------|----------|-------------------|-------------------|
| var | Function Scope | Yes | Yes | Yes |
| let | Block scope | No | Yes | No |
| const | Block scope | No | No | No |

***Arrow functions***

The arrow function expression syntax is a shorter way of creating a function expression. Arrow functions do not have their own this, do not have prototypes, cannot be used for constructors, and should not be used as object methods.


--- 
## React

### ***Why JSX ?***

React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.


### ***Rendering an Element into the DOM***

Let’s say there is a <div> somewhere in your HTML file :

    <div id="root"></div>

We call this a “root” DOM node because everything inside it will be managed by React DOM.

Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

To render a React element into a root DOM node, pass both to ReactDOM.render():


    const element = <h1>Hello, world</h1>;
    ReactDOM.render(element, document.getElementById('root'));


Try it on CodePen

It displays “Hello, world” on the page.

### ***Props***

Whether you declare a component as a function or a class, it must never modify its own props. Consider this sum function:

    function sum(a, b) {
        return a + b;
    }

Such functions are called “pure” because they do not attempt to change their inputs, and always return the same result for the same inputs.

In contrast, this function is impure because it changes its own input:

    function withdraw(account, amount) {
        account.total -= amount;
    }

React is pretty flexible but it has a single strict rule:

All React components must act like pure functions with respect to their props.

Of course, application UIs are dynamic and change over time.


### ***Handling Events***

Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences :

- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

---
## Tailwind CSS

***Why not just use inline styles ?***

A common reaction to this approach is wondering, “isn’t this just inline styles?” and in some ways it is — you’re applying styles directly to elements instead of assigning them a class name and then styling that class.

But using utility classes has a few important advantages over inline styles:

**Designing with constraints.**

Using inline styles, every value is a magic number. With utilities, you’re choosing styles from a predefined design system, which makes it much easier to build visually consistent UIs.

**Responsive design.**

You can’t use media queries in inline styles, but you can use Tailwind’s responsive utilities to build fully responsive interfaces easily.

**Hover, focus, and other states.**

Inline styles can’t target states like hover or focus, but Tailwind’s state variants make it easy to style those states with utility classes

---
## Next.js

To build a complete web application with React from scratch, there are many important details you need to consider:

- Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
- You need to do production optimizations such as code splitting.
- You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
- You might have to write some server-side code to connect your React app to your data store.


***Next.js: The React Framework***

Enter Next.js, the React Framework. Next.js provides a solution to all of the above problems. But more importantly, it puts you and your team in the pit of success when building React applications.

Next.js aims to have best-in-class developer experience and many built-in features, such as:

- An intuitive page-based routing system (with support for dynamic routes)
- Pre-rendering, both static generation (SSG) and server-side rendering (SSR) are supported on a per-page basis
- Automatic code splitting for faster page loads
- Client-side routing with optimized prefetching
- Built-in CSS and Sass support, and support for any CSS-in-JS library
- Development environment with Fast Refresh support
- API routes to build API endpoints with Serverless Functions
- Fully extendable

Next.js is used in tens of thousands of production-facing websites and web applications, including many of the world's largest brands.

---
## Sources and references

- ***[ES6 Syntax and Feature Overview .](https://www.taniarascia.com/es6-syntax-and-feature-overview/)***

- ***[React - Hello World .](https://reactjs.org/docs/hello-world.html)***

- ***[React - JSX .](https://reactjs.org/docs/introducing-jsx.html)***

- ***[React - Rendering Elements .](https://reactjs.org/docs/rendering-elements.html)***

- ***[React - Components & Props .](https://reactjs.org/docs/components-and-props.html)***

- ***[React - State & Lifecycle .](https://reactjs.org/docs/state-and-lifecycle.html)***

- ***[React - Handling Events .](https://reactjs.org/docs/handling-events.html)***

- ***[Utility First CSS .](https://tailwindcss.com/docs/utility-first)***

- ***[Tailwind in 15 minutes .](https://www.youtube.com/watch?v=6zIuAyLZPH0)***

- ***[Learn Next.js .](https://nextjs.org/learn/basics/create-nextjs-app)***

- ***[Why to use Next.js .](https://www.youtube.com/watch?v=rtgbaKBhdkk)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

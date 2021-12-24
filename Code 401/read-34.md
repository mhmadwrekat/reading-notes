# Pythonisms

---
## Dunder Methods

***What Are Dunder Methods ?***

In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __init__ or __str__.

As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”

These “dunders” or “special methods” in Python are also sometimes called “magic methods.” But using this terminology can make them seem more complicated than they really are—at the end of the day there’s nothing “magical” about them. You should treat these methods like a normal language feature.


Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box :

    class NoLenSupport:
        pass
    >>> obj = NoLenSupport()
    >>> len(obj)
    TypeError: "object of type 'NoLenSupport' has no len()"

To fix this, you can add a __len__ dunder method to your class :

    class LenSupport:
        def __len__(self):
            return 42
    >>> obj = LenSupport()
    >>> len(obj)
    42

Another example is slicing. You can implement a __getitem__ method which allows you to use Python’s list slicing syntax: obj[start:stop].

---
## Iterators

Understanding iterators is a milestone for any serious Pythonista. With this step-by-step tutorial you’ll understanding class-based iterators in Python, completely from scratch.

I love how beautiful and clear Python’s syntax is compared to many other programming languages.

Let’s take the humble for-in loop, for example. It speaks for Python’s beauty that you can read a Pythonic loop like this as if it was an English sentence:

    numbers = [1, 2, 3]
    for n in numbers:
        print(n)

But how do Python’s elegant loop constructs work behind the scenes ? 

How does the loop fetch individual elements from the object it is looping over?

And how can you support the same programming style in your own Python objects?


You’ll find the answer to these questions in Python’s iterator protocol :

Objects that support the __iter__ and __next__ dunder methods automatically work with for-in loops.

But let’s take things step by step. Just like decorators, iterators and their related techniques can appear quite arcane and complicated on first glance. So we’ll ease into it.

In this tutorial you’ll see how to write several Python classes that support the iterator protocol. They’ll serve as “non-magical” examples and test implementations you can build upon and deepen your understanding with.

We’ll focus on the core mechanics of iterators in Python 3 first and leave out any unnecessary complications, so you can see clearly how iterators behave at the fundamental level.


![python loop](https://ipcisco.com/wp-content/uploads/2021/03/python-for-loop-ipcisco-3.jpg)

---
## Generators

If you’ve ever implemented a class-based iterator from scratch in Python, you know that this endeavour requires writing quite a bit of boilerplate code.

And yet, iterators are so useful in Python: They allow you to write pretty for-in loops and help you make your code more Pythonic and efficient.

As a (proud) “lazy” Python developer, I don’t like tedious and repetitive work. And so, I often found myself wondering:

If there only was a more convenient way to write these Python iterators in the first place…

Surprise, there is! Once again, Python helps us out with some syntactic sugar to make writing iterators easier.


Let’s start by looking again at the Repeater example that I previously used to introduce the idea of iterators. It implemented a class-based iterator cycling through an infinite sequence of values.

This is what the class looked like in its second (simplified) version :


    class Repeater:
        def __init__(self, value):
            self.value = value
        def __iter__(self):
            return self
        def __next__(self):
            return self.value


If you’re thinking, “that’s quite a lot of code for such a simple iterator,” you’re absolutely right. Parts of this class seem rather formulaic, as if they would be written in exactly the same way from one class-based iterator to the next.

This is where Python’s generators enter the scene. If I rewrite this iterator class as a generator, it looks like this:

    def repeater(value):
        while True:
            yield value

***We just went from seven lines of code to three.***

---
## Sources and references

- ***[Dunder Methods .](https://dbader.org/blog/python-dunder-methods)***

- ***[Iterators .](https://dbader.org/blog/python-iterators)***

- ***[Generators .](https://dbader.org/blog/python-generators)***

- ***[What are Generators .](https://realpython.com/lessons/what-are-python-generators/)***

- ***[Decorators .](https://realpython.com/primer-on-python-decorators/)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

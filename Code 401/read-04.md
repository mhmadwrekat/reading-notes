# Classes, Objects, Thinking Recursively, Pytest

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Classes and Objects|First Paragraph|
|Thinking Recursively|Second Paragraph|
|Pytest Fixtures and Coverage|Third Paragraph|

---
## Classes and Objects

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects .

**Example**

    class MyClass:
        variable = "blah"

        def function(self):
            print("This is a message inside the class.")


**Accessing Object Functions**

To access a function inside of an object you use notation similar to accessing a variable :

    class MyClass:
        variable = "blah"

        def function(self):
            print("This is a message inside the class.")

    myobjectx = MyClass()

    myobjectx.function()


![Classes and Objects](https://freetutsdownload.net/wp-content/uploads/2019/01/4c5684c4-2074920_20c7_4.jpg)

---
## Thinking Recursively

*“Of all ideas I have introduced to children, recursion stands out as the one idea that is particularly able to evoke an excited response.”*

Problems (in life and also in computer science) can often seem big and scary. But if we keep chipping away at them, more often than not we can break them down into smaller chunks trivial enough to solve. This is the essence of thinking recursively .

Recursive Functions in Python
Now that we have some intuition about recursion, let’s introduce the formal definition of a recursive function. A recursive function is a function defined in terms of itself via self-referential expressions .


This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: ***base case*** and ***recursive case*** .

### Maintaining State
When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either :

* Thread the state through each recursive call so that the current state is part of the current call’s execution context .

* Keep the state in global scope .


![Thinking Recursively](https://files.realpython.com/media/Thinking-Recursively-in-Python_Watermarked.1825397c00ea.jpg)

---
## Pytest Fixtures and Coverage

**Fixtures**

When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests" .


**Coverage**

if you've ever done any testing, you know there's always the question of how thoroughly you have tested your code. After all, let's say you've written five functions, and that you've written tests for all of them. Can you be sure you've actually tested all of the possible paths through those functions?

*For example, let's assume you have a very strange function, only_odd_mul, which multiplies only odd numbers :*

    def only_odd_mul(x, y):
    if x%2 and y%2:
           return x * y
    else:
           raise NoEvenNumbersHereException(f'{x} and/or {y}
       not odd')


*Here's a test you can run on it:*


    def test_odd_numbers():
        assert only_odd_mul(3, 5) == 15


![Pytest Fixtures and Coverage](https://files.realpython.com/media/Getting-Started-with-Testing-in-Python_Watermarked.9f22be97343d.jpg)

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>



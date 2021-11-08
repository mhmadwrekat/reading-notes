# Game of Greed **3**

---
## List Comprehensions

- List comprehension methods are an elegant way to create and manage lists . 

- In Python, list comprehensions are a more compact way of creating lists . 

- More flexible than for loops, list comprehension is usually faster than other methods .


**Create a List Using Loops and List Comprehension in Python**

To better illustrate how a list comprehension can be used to write more efficient Python code, we’ll take a look at a side by side comparison. 

In the following example, you’ll see two different techniques for creating a Python list. The first is a for loop. We’ll use it to construct a list of the powers of two.

Example 2: Comparing list creation methods in Python

First, create a list and loop through it. Add an expression, in this example, we’ll raise x to the power of 2.


    squares = []

    for x in range(10):
        # raise x to the power of 2
        squares.append(x**2)

    print(squares)
    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]


**Output**

The same thing can be done using a list comprehension, but with a fraction of the code. Let’s take a look at how to create a list of squares using the list comprehension method.

    squares = [x**2 for x in range(10)]

    print(squares)


Even in this basic example, it’s obvious that list comprehensions reduce the code necessary to complete rather complicated task when working with a list.

---
**Lower/Upper case converter using Python**

Using list comprehension to loop through a string in Python, it’s possible to convert strings from lower case to upper case, and vice versa. 

Making use of Python’s lower() and upper() methods, we’ll use list comprehension to achieve this common task.

    lower_case = [ letter.lower() for letter in ['A','B','C'] ]
    upper_case = [ letter.upper() for letter in ['a','b','c'] ]

    print(lower_case, upper_case)


**Output**

    ['a', 'b', 'c'] ['A', 'B', 'C']


![List Comprehensions](https://cdn.educba.com/academy/wp-content/uploads/2019/11/list-comprehensions-python.png)

---

#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
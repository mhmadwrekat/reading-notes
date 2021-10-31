# Testing and Modules

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|In Tests We Trust - TDD with Python|First Paragraph|
|If name equals main|Second Paragraph|
|Recursion|Third Paragraph|

---
## In Tests We Trust - TDD with Python

**TDD is not about the money/tests**

More than any checking, we need to think about our software design first.
One of the things that amaze me about TDD is how we can grow our software design consciously and well, just building what is needed to make the test pass. When we are writing tests we are forced to think about the design first and how we can break it into small pieces.

Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

But Test-Driven Development is a strategy to think (and write!) tests first.


* The cycle is made by three steps:

1. Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)

2. Write the feature and make the test pass! (you can dance after that)

3. Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)

![TDD](https://miro.medium.com/max/2000/1*KmwA_4r6wICrF1jc9bx4dg.png)


---
## If name equals main

**What does the if __name__ == “__main__”: do ?**

If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable .

**Why Do we need it ?**

Advantages : 

1. Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.

2. If you import this script as a module in another script, the __name__ is set to the name of the script/module.

3. Python files can act as either reusable modules, or as standalone programs.

4. if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported .


---
## Recursion

**What is Recursion ?** 

The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily. Examples of such problems are Towers of Hanoi (TOH), Inorder/Preorder/Postorder Tree Traversals, DFS of Graph, etc .

**How a particular problem is solved using recursion ?** 

The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion. For example, we compute factorial n if we know factorial of (n-1). The base case for factorial would be n = 0. We return 1 when n = 0. 

![recursion](https://i.ytimg.com/vi/ixdr6V2vRC4/maxresdefault.jpg)

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

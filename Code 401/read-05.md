# Linked Lists

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Quiz|First Paragraph|
|Big O: Analysis of Algorithm Efficiency|Second Paragraph|
|Linked Lists|Third Paragraph|
|Answers|Last Paragraph|

---
## Quiz

1. different betweeen *Worst Case, Best Case, Average Case* ?
2. what is Big Omega ?
3. what is Running Time ?
4. What is a Linked List ?

---
## Big O: Analysis of Algorithm Efficiency 

Big O(oh) notation is used to describe the efficiency of an algorithm or function. This efficiency is evaluated based on 2 factors:

1. Running Time (also known as time efficiency / complexity)
The amount of time a function needs to complete.

2. Memory Space (also known as space efficiency / complexity)
The amount of memory resources a function uses to store data and instructions.

Big O’s role in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job. It specifically looks at the factors mentioned above, which we often refer to as Space and Time. In order to analyze these limiting factors, we should consider 4 Key Areas for analysis:

1. Input Size
2. Units of Measurement
3. Orders of Growth
4. Best Case, Worst Case, and Average Case


*Orders of Growth*

We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n. As the value of n grows, the Order of Growth represents the increase in Running Time or Memory Space.

*Worst Case, Best Case, Average Case*

Even though Big O describes the Worst Case for algorithm efficiency, we can still think about Best and Average cases. Each of these cases could be analyzed as we consider the overall question: As inputs n fluctuate in size and order, how does this affect our orders of Growth?

Worst Case: The efficiency for the worst possible input of size n
This case runs the longest for all possible inputs of n. This assumes that if we were sorting values, inputs are completely unsorted and searched values either don’t exist or are at the last to be searched.

Best Case: The efficiency for the best possible input of size n
This case runs the quickest for all possible inputs of n. In the case of sorting, this assumes that values are sorted, and so searched-for values are easy to find.

Average Case: The efficiency for a “typical” or “random” input of size n.
The average case makes a typical assumption about the possible inputs of size ‘n’ and how they might affect efficiency. This is NOT the best case and worst case averaged together.


- Big O: The worst case analysis of algorithm efficiency.
- Running Time: The amount of time required for an algorithm to complete.
- Memory Space: The amount of memory resources required for an algorithm to complete.
- Input Size: Represented by the variable n, the total size of values used as parameters in an algorithm.
- Big Omega: The best case analysis of algorithm efficiency.
- Big Theta: The typical or random case used for analysis of algorithm efficiency.


![Big O](https://www.educative.io/v2api/editorpage/6522953121398784/image/5162949189566464)

---
## Linked Lists

A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

There are two types of Linked List - **Singly** and **Doubly**. We will be implementing a Singly Linked List in this implementation.

*Prerequisites*

When constructing your code, a few things to keep in mind.

When making your Node class, consider requiring a value to be passed in to require that each node has a value.

*Linear data structures*

If we really want to understand the basics of linked lists, it’s important that we talk about what type of data structure they are.


One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. We can think of a linear data structure like a game of hopscotch: in order to get to the end of the list, we have to go through all of the items in the list in order, or sequentially. Linear structures, however, are the opposite of non-linear structures. In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

**A good rule of thumb for remember the characteristics of linked lists is this:**

    a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.

![Linked Lists](https://files.realpython.com/media/Python-Linked-Lists-Guide_Watermarked.421631d9a615.jpg)

---
## Answers 
1. 
* Worst Case: The efficiency for the worst possible input of size n
    This case runs the longest for all possible inputs of n. This assumes that if we were sorting values, inputs are completely unsorted and searched values either don’t exist or are at the last to be searched.

* Best Case: The efficiency for the best possible input of size n
    This case runs the quickest for all possible inputs of n. In the case of sorting, this assumes that values are sorted, and so searched-for values are easy to find.

* Average Case: The efficiency for a “typical” or “random” input of size n.
    The average case makes a typical assumption about the possible inputs of size ‘n’ and how they might affect efficiency. This is NOT the best case and worst case averaged together.

2. Big Omega: The best case analysis of algorithm efficiency .

3. Running Time: The amount of time required for an algorithm to complete.

4. Linked Lists : A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link , There are two types of Linked List - **Singly** and **Doubly**. We will be implementing a Singly Linked List in this implementation.

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>



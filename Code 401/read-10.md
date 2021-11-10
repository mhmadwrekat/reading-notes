# Stacks and Queues

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Quiz|First Paragraph|
|Stacks|Second Paragraph|
|Queues|Third Paragraph|
|Answers|Last Paragraph|

---
## Quiz

1. What is a Stack ?
2. What is a Queue ?
3. what's the concepts Queues follow them ?
4. what's the concepts Stacks follow them ?
5. Common terminology for a stack is ?

---
## Stacks and Queues

**What is a Stack**

A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous .


**Push O(1)**

Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.


**Common terminology for a stack is**

1. **Push** - Nodes or items that are put into the stack are pushed
2. **Pop** - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
3. **Top** - This is the top of the stack.
4. **Peek** - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
5. **IsEmpty** - returns true when stack is empty otherwise returns false.


**Peek O(1)**
When conducting a peek, you will only be inspecting the top Node of the stack.

Typically, you would check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

Here is the pseudocode for a peek


    ALGORITHM peek()
    // INPUT <-- none
    // OUTPUT <-- value of top Node in stack
    // EXCEPTION if stack is empty

       return top.value

We do not re-assign the next property when we peek because we want to keep the reference to the next Node in the stack. This will allow the top to stay the top until we decide to pop.

**Stacks follow these concepts:**

- FILO
First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

- LIFO
Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack

---
## Queue

**What is a Queue**
*Common terminology for a queue is*

1. **Enqueue** - Nodes or items that are added to the queue.
2. **Dequeue** - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. **Front** - This is the front/first Node of the queue.
4. **Rear** - This is the rear/last Node of the queue.
5. **Peek** - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. **IsEmpty** - returns true when queue is empty otherwise returns false.


**Queues follow these concepts:**

- FIFO
First In First Out

This means that the first item in the queue will be the first item out of the queue.

- LILO
Last In Last Out

This means that the last item in the queue will be the last item out of the queu .


**Peek O(1)**
When conducting a peek, you will only be inspecting the front Node of the queue.

Typically, you want to check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

*Code*
Here is the pseudocode for a peek

    ALGORITHM peek()
    // INPUT <-- none
    // OUTPUT <-- value of the front Node in Queue
    // EXCEPTION if Queue is empty

       return front.value
We do not re-assign the next property when we peek because we want to keep the reference to the next Node in the queue. This will allow the front to stay in the front until we decide to dequeue

![Stacks and Queues](https://qph.fs.quoracdn.net/main-qimg-24bca798c3f39527d91bc325da651b68)

---
## Answers 

1. **What is a Stack ?**
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous .


2. **What is a Queue ?**
*Common terminology for a queue is*

- **Enqueue** - Nodes or items that are added to the queue.
- **Dequeue** - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
- **Front** - This is the front/first Node of the queue.
- **Rear** - This is the rear/last Node of the queue.
- **Peek** - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
- **IsEmpty** - returns true when queue is empty otherwise returns false.


3. **what's the concepts Queues follow them ?**

**Queues follow these concepts:**

- FIFO
First In First Out

This means that the first item in the queue will be the first item out of the queue.

- LILO
Last In Last Out

This means that the last item in the queue will be the last item out of the queu .


4. **what's the concepts Stacks follow them ?**

**Stacks follow these concepts:**

- FILO
First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

- LIFO
Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack


5. **Common terminology for a stack is**

1. **Push** - Nodes or items that are put into the stack are pushed
2. **Pop** - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
3. **Top** - This is the top of the stack.
4. **Peek** - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
5. **IsEmpty** - returns true when stack is empty otherwise returns false.

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
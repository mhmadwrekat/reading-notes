# Big O & Python

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Beginners Guide to Big O|First Paragraph|
|Names and Values in Python|Second Paragraph|
|lovers of reading|Third Paragraph|
|Things I want to know more about|In The Last|

---
## Beginners Guide to Big O

The best way to understand Big O thoroughly was to produce some examples in code. So, below are some common orders of growth along with descriptions and examples where possible.

#### **O(1)**

**O(1)** describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

    bool IsFirstElementNull(IList<String> elements)
    {
        return elements[0] == null;
    }

#### **O(N)**
O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set. The example below also demonstrates how Big O favours the worst-case performance scenario; a matching string could be found during any iteration of the for loop and the function would return early, but Big O notation will always assume the upper limit where the algorithm will perform the maximum number of iterations.

    bool ContainsValue(IEnumerable<string> elements, string value)
    {
        foreach (var element in elements)
        {
            if (element == value) return true; 
        }     
        return false; 
    }

#### **O(N²)**
O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N³), O(N⁴) etc.

    bool ContainsDuplicates(IList<string> elements)
    {
        for (var outer = 0; outer < elements.Count; outer++) 
        {
            for (var inner = 0; inner < elements.Count; inner++) 
            {   
                // Don't compare with self 
                if (outer == inner) continue;             
            
                if (elements[outer] == elements[inner]) return true; 
            }
        }    
        return false;
    }

#### **O(2^N)**
O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. The growth curve of an O(2^N) function is exponential — starting off very shallow, then rising meteorically. An example of an O(2^N) function is the recursive calculation of Fibonacci numbers:

    int Fibonacci(int number)
    {
        if (number <= 1) return number;
       
        return Fibonacci(number - 2) + Fibonacci(number - 1); 
    }

![big O](https://www.educative.io/v2api/editorpage/6522953121398784/image/5162949189566464)


#### **Logarithms**

Logarithms are slightly trickier to explain so I’ll use a common example:

Binary search is a technique used to search sorted data sets. It works by selecting the middle element of the data set, essentially the median, and compares it against a target value. If the values match, it will return success. If the target value is higher than the value of the probe element, it will take the upper half of the data set and perform the same operation against it. Likewise, if the target value is lower than the value of the probe element, it will perform the operation against the lower half. It will continue to halve the data set with each iteration until the value has been found or until it can no longer split the data set.

---
## Names and Values in Python

Python’s variables are names that refer to values. Names have no type, and there are no variable declarations. Names are created by assigning a value to them:

**x = "value"**

![Python](https://cdn.analyticsvidhya.com/wp-content/uploads/2021/07/38787wallpaper.png)

All values in Python are objects (more about that later). Every value has a definite type.

*Because names are not typed, they can be assigned new values with a different type than their old value :*

> x = 1

> x = "hello"     # This is fine.

### ***Python has a rich set of built-in types :***

* Numbers, including unlimited precision integers, double-precision floats, and complex numbers.

* Booleans, with constants True and False.

* A special value, None, used when no other value is appropriate.

* Strings, both byte strings and Unicode strings (see Strings).

* Containers like lists (see Lists) and dictionaries (see Dictionaries).

* User-defined objects (see Classes).

In addition to these conventional data types, in Python many things that you might not expect are first-class values, like functions, classes, and modules. These can be manipulated just like other values, assigning them to names, passing them to functions, and storing them in containers .

---
## ***For lovers of reading*** :

<img src='https://www.lovereading.co.uk/content/images/love-reading-generic-facebook-image.jpg' height='300'>


**[More about Awesome Python Environment ......](https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5?gi=6a6c1f098521)**

**[More about Python Module of the Week ......](https://pymotw.com/3/index.html)**

---
## Things I want to know more about

* ### ***In Tests We Trust - TDD with Python .***

* ### ***If name equals main .***

* ### ***Recursion .***

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>

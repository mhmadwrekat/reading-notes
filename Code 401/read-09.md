# Game of Greed **4**

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Dunder Methods|First Paragraph|
|Statistics - Probability|Second Paragraph|
|Statistics Module|Last Paragraph|

---
## Dunder Methods

***What Are Dunder Methods?***

In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __ init __ or __ str __ .


As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”


These “dunders” or “special methods” in Python are also sometimes called “magic methods.” But using this terminology can make them seem more complicated than they really are—at the end of the day there’s nothing “magical” about them. You should treat these methods like a normal language feature.

Object Representation: __ str __ , __ repr __
It’s common practice in Python to provide a string representation of your object for the consumer of your class (a bit like API documentation.) There are two ways to do this using dunder methods:

1. __ repr __ : The “official” string representation of an object. This is how you would make an object of the class. The goal of __ repr __ is to be unambiguous.

2. __ str __ : The “informal” or nicely printable string representation of an object. This is for the enduser.



![Dunder Methods](https://holycoders.com/content/images/wordpress/2020/03/Python-Tutorial-dunder-or-special-methods.png)

---
## Statistics - Probability

***What is probability ?***

At the most basic level, probability seeks to answer the question, “What is the chance of an event happening?” An event is some outcome of interest. To calculate the chance of an event happening, we also need to consider all the other events that can occur. The quintessential representation of probability is the humble coin toss. In a coin toss the only events that can happen are:

1. Flipping a heads .
2. Flipping a tails .


These two events form the sample space, the set of all possible events that can happen. To calculate the probability of an event occurring, we count how many times are event of interest can occur (say flipping heads) and dividing it by the sample space. Thus, probability will tell us that an ideal coin will have a 1-in-2 chance of being heads or tails. By looking at the events that can occur, probability gives us a framework for making predictions about how often events will happen. However, even though it seems obvious, if we actually try to toss some coins, we’re likely to get an abnormally high or low counts of heads every once in a while. If we don’t want to make the assumption that the coin is fair, what can we do? We can gather data! We can use statistics to calculate probabilities based on observations from the real world and check how it compares to the ideal.


![Statistics - Probability](https://i.ytimg.com/vi/9MjQCGbyHws/maxresdefault.jpg)

---
## Statistics Module

The module is not intended to be a competitor to third-party libraries such as NumPy, SciPy, or proprietary full-featured statistics packages aimed at professional statisticians such as Minitab, SAS and Matlab. It is aimed at the level of graphing and scientific calculators.

**Measures of spread**

These functions calculate a measure of how much the population or sample tends to deviate from the typical or average values.


**Function details**
Note: The functions do not require the data given to them to be sorted. However, for reading convenience, most of the examples show sorted sequences.

***statistics.mean(data)***
Return the sample arithmetic mean of data which can be a sequence or iterable.

The arithmetic mean is the sum of the data divided by the number of data points. It is commonly called “the average”, although it is only one of many different mathematical averages. It is a measure of the central location of the data.

If data is empty, StatisticsError will be raised.

*Some examples of use:*

    >>>
    >>> mean([1, 2, 3, 4, 4])
    2.8
    >>> mean([-1.0, 2.5, 3.25, 5.75])
    2.625

    >>> from fractions import Fraction as F
    >>> mean([F(3, 7), F(1, 21), F(5, 3), F(1, 3)])
    Fraction(13, 21)

    >>> from decimal import Decimal as D
    >>> mean([D("0.5"), D("0.75"), D("0.625"), D("0.375")])
    Decimal('0.5625')


---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
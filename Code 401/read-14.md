# Data Visualization

***Matplotlib Tutorial***
matplotlib is probably the single most used Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats .

**IPython**
IPython is an enhanced interactive Python shell that has lots of interesting features including named inputs and outputs, access to shell commands, improved debugging and much more. It allows interactive matplotlib sessions that have Matlab/Mathematica-like functionality .

**pyplot**
pyplot provides a convenient interface to the matplotlib object-oriented plotting library. It is modeled closely after Matlab(TM). Therefore, the majority of plotting commands in pyplot have Matlab(TM) analogs with similar arguments. Important commands are explained with interactive examples .

---
***Setting tick labels***

Documentation

- Working with text
- xticks() command
- yticks() command
- set_xticklabels()
- set_yticklabels()

***Moving spines***

Documentation

- Spines
- Axis container
- Transformations tutorial

---
## Figures, Subplots, Axes and Ticks
implicit figure and axes creation. This is handy for fast plots. We can have more control over the display using figure, subplot, and axes explicitly. A figure in matplotlib means the whole window in the user interface. Within this figure there can be subplots. While subplot positions the plots in a regular grid, axes allows free placement within the figure. Both can be useful depending on your intention. We've already worked with figures and subplots without explicitly calling them. When we call plot, matplotlib calls gca() to get the current axes and gca in turn calls gcf() to get the current figure. If there is none it calls figure() to make one, strictly speaking, to make a subplot(111). 

![Data Visualization](https://www.dataflareup.com/wp-content/uploads/2021/10/data-visualization-trends.jpg)

---
***Simple plot***
In this section, we want to draw the cosine and sine functions on the same plot. Starting from the default settings, we'll enrich the figure step by step to make it nicer.

The first step is to get the data for the sine and cosine functions:

    import numpy as np

    X = np.linspace(-np.pi, np.pi, 256, endpoint=True)
    C, S = np.cos(X), np.sin(X)

X is now a NumPy array with 256 values ranging from -π to +π (included). C is the cosine (256 values) and S is the sine (256 values).

To run the example, you can download each of the examples and run it using:

    $ python exercice_1.py

You can get source for each step by clicking on the corresponding figure.

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
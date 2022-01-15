# Scenario

It's your second week as a data analyst at PyBer, a ride-sharing app company valued at $2.3 billion. You've just been assigned your first big project: **analyze all the rideshare data from January to early May of 2019 and create a compelling visualization for the CEO, V. Isualize.**

Even before starting at PyBer, you'd heard stories about V. Isualize. She is a former programmer who started out at MathWorks, a co-founder of PyBer, and is known for being extremely fair yet extremely demanding. Because of her programming expertise, she's particularly insistent that the analytical work be comprehensive and correct. This assignment is both a once-in-a-lifetime challenge and a once-in-a-lifetime opportunity. If you do well, your future at the organization is secure.

Your manager, Omar, is excited for your big break and has agreed to partner with you on getting the visualizations just right. Your first step is to create a GitHub repository for the project so that he can stay in the loop as you work.

## 5.1.2

You've just received the work assignment of a lifetime: creating visualizations of rideshare data for PyBer to help improve access to ride-sharing services and determine affordability for underserved neighborhoods. As a new employee, this is a huge professional opportunity for you!

The first step is to make sure you have the right tools in place. A simple Excel chart isn't going to impress V. Isualize. Instead, you'll use the Python graphing library Matplotlib, which is a favorite tool among data scientists and data analysts because of its robust visualization features.

Omar has given you some backstory about the connection between V. Isualize and Matplotlib. Matplotlib was created as a Python alternative for MATLAB. MATLAB, which is short for matrix laboratory, was developed by the company MathWorks in the 1980s. It enabled scientists to perform linear algebra and numerical analysis without learning the programming language Fortran, which until then had been the best option for complex computations.

With this information, you realize that the CEO is an expert in creating data visualizations. You definitely can't afford to botch this up!

# Matplotlib Intro

`%matplotlib inline`

The `%` sign is sometimes called the magic command. When you run a cell that starts with %, "magic" happens behind the scenes and **sets the back-end processor used for charts**. Using it with the `inline` value displays the chart within the cell for a Jupyter Notebook file.

## Object Oriented Explanation:

```python
# Create the plot with ax.plt()
fig, ax = plt.subplots()
ax.plot(x_axis, y_axis)
```

Let's break down what the code is doing:

- The `plt.subplots()` function returns a tuple that contains a figure and axes object(s).
- `fig, ax = plt.subplots()` unpacks the tuple into the variables `fig` and `ax`.
- The first variable, `fig`, references the figure.
- The second variable, `ax`, references the axes of the figure and allows us to annotate the figure.
- The `ax.plot(x_axis, y_axis)` plots the data from the x and y axes.

```python
# Create the plot with ax.plt()
fig = plt.figure()
ax = fig.add_subplot()
```
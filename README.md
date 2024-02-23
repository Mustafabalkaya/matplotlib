```markdown
# Graph Drawing with Matplotlib

In this project, we utilized the `matplotlib` library to perform basic drawing operations. Additionally, we read data from a CSV file and applied various graph features.

## Basic Drawing Operations

We used the `matplotlib` library for graph drawing operations. A simple drawing example is as follows:

```python
import matplotlib.pyplot as plt

# Define the data
x = [1, 2, 3, 4, 5]
y = [10, 20, 15, 25, 30]

# Perform the drawing
plt.plot(x, y, label='Dataset 1')

# Add graph features
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Basic Drawing Operations')
plt.legend()

# Show the plot
plt.show()
```

## Adding a Legend

To add a legend when displaying multiple plots on the same graph, we used the `legend()` function. For example:

```python
# Perform the drawing
plt.plot(x, y, label='Dataset 1')
plt.plot(x, [i*2 for i in y], label='Dataset 2')

# Add a legend
plt.legend()

# Show the plot
plt.show()
```

## Drawing Multiple Plots on the Same Graph

You can display multiple plots on the same graph by using the `plot()` function and drawing each plot separately.

## Saving the Graph to Your Computer

To save the created graph to your computer, you can use the `savefig()` function. For example:

```python
plt.savefig('graph.png')
```

## Bar Chart

To draw a bar graph, you can use the `bar()` function. For example:

```python
# Define the data
categories = ['A', 'B', 'C', 'D']
values = [30, 50, 20, 40]

# Draw a bar graph
plt.bar(categories, values, color='blue')

# Show the plot
plt.show()
```

## Example with Oil Prices

Within the project, we read data from the `petrolfiyatlari.csv` file and created a graph. Sample code:

```python
import pandas as pd

# Read the CSV file
data = pd.read_csv('petrolfiyatlari.csv')

# Draw the data
plt.plot(data['Date'], data['Brent'], label='Brent Crude Oil')
plt.plot(data['Date'], data['WTI'], label='WTI Crude Oil')

# Add graph features
plt.xlabel('Date')
plt.ylabel('Price ($)')
plt.title('Oil Prices')
plt.legend()

# Show the plot
plt.show()
```

## Figure Size

To set the size of the drawings, you can use the `figure()` function. For example:

```python
# Set the figure size
plt.figure(figsize=(10, 6))

# Perform other drawing operations
# ...

# Show the plot
plt.show()
```

These steps cover various topics, from basic drawing operations to adding a legend, displaying multiple plots on the same graph, saving the graph, drawing a bar chart, reading data, and setting a custom figure size. You can add this README file to the root directory of your project to provide users with a guide on how to use your project.
```

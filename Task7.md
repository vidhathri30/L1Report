
## TASk 7
**Curve fitting**

Curve fitting is an optimization problem that finds a line that best fits a collection of observations.

It is easiest to think about curve fitting in two dimensions, such as a graph.

Consider that we have collected examples of data from the problem domain with inputs and outputs.

The x-axis is the independent variable or the input to the function. The y-axis is the dependent variable or the output of the function. We don’t know the form of the function that maps examples of inputs to outputs, but we suspect that we can approximate the function with a standard function form.

Curve fitting involves first defining the functional form of the mapping function (also called the basis function or objective function), then searching for the parameters to the function that result in the minimum error.

The key to curve fitting is the form of the mapping function.

A straight line between inputs and outputs can be defined as follows:

**y = a * x + b**

Where y is the calculated output, x is the input, and a and b are parameters of the mapping function found using an optimization algorithm.

In a linear regression model, these parameters are referred to as coefficients; in a neural network, they are referred to as weights.

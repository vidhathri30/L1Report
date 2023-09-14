
## TASk 7
## Curve fitting

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

![Screenshot 2023-09-14 152300](https://github.com/vidhathri30/L1Report/assets/101579638/e0e457b0-ad22-4bf9-a4d1-7aea46c9bf56)
![Screenshot 2023-09-14 152317](https://github.com/vidhathri30/L1Report/assets/101579638/1444788b-e36e-4d5b-a63f-b220300df623)

 ## Fourier Transforms usng MATLAB

 Fourier Transform is a mathematical technique that helps to transform Time Domain function x(t) to Frequency Domain function X(ω).

 The mathematical expression for Fourier transform is:X(ω) = F\{x(t)\} = ∫_{-∞}^∞x(t).e^{(-jωt)} dt

 Using the above function one can generate a Fourier Transform of any expression. In MATLAB, the Fourier command returns the Fourier transform of a given function.

 1.Creating a synthesised signal

![Screenshot 2023-09-14 154129](https://github.com/vidhathri30/L1Report/assets/101579638/2a0e25ab-dc0d-4a50-bbc7-595f9b459e2a)
![Screenshot 2023-09-14 154151](https://github.com/vidhathri30/L1Report/assets/101579638/1109e9d7-2457-45cf-b8c1-6e34633cac59)


 2.Using FFT to analyze the signal
do?
A fast Fourier transform (FFT) is a highly optimized implementation of the discrete Fourier transform (DFT), which convert discrete signals from the time domain to the frequency domain. FFT computations provide information about the frequency content, phase, and other properties of the signal.

![Screenshot 2023-09-14 154415](https://github.com/vidhathri30/L1Report/assets/101579638/27c39541-c6c5-4458-874f-59b221760c40)
![Screenshot 2023-09-14 154426](https://github.com/vidhathri30/L1Report/assets/101579638/86949b5f-2fe9-4ebf-a124-11d7977954c3)


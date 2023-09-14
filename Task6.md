
## Neural Networks:

Neural networks have revolutionized the field of artificial intelligence and machine learning. They are at the core of many modern applications, from image recognition to natural language processing. a neural network is a computational model inspired by the structure and function of the human brain. It consists of interconnected nodes, known as neurons, organized into layers. These layers typically include an input layer, one or more hidden layers, and an output layer.

Types of neural network are:

Perceptron
Feed Forward Neural Network
Multilayer Perceptron
Convolutional Neural Network
Radial Basis Functional Neural Network
Recurrent Neural Network
LSTM – Long Short-Term Memory
Sequence to Sequence Models
Modular Neural Network



## Artificial neural networks (ANN)

Artificial neural networks (ANN) are nonlinear mathematical tools intended for simulating human brain processing through simple units called artificial neurons arranged
in structures known as layers. They are widely used in many branches of science with
high potential in classification/pattern recognition or regression tasks. Similarly to the
human cognitive processes, their abilities include forecasting and learning operations. In
ANN contexts, learning is often referred to as training

The connection between one unit from input layer and one from hidden layer is represented by a number called a weight, which is denoted as Wi. The
weight can be either positive or negative, which corresponds to the way
actual brain cells excite or suppress others.

1.Considering we have data and would like to apply binary classification to get the desired output. 

2.Take a sample having features as X1, X2, and these features will be operated over a set of processes to predict the outcome.

3.Each feature is associated with a weight, where X1, X2 as features and W1, W2 as weights. These are served as input to a neuron.

4.In the summation, all features are multiplied by their weights and bias are summed up. (Y=W1X1+W2X2+b).
![Screenshot 2023-09-14 132110](https://github.com/vidhathri30/L1Report/assets/101579638/54022c4e-88d4-4b8a-ad83-650f46e402c7)




## Convolutional Neural Network (CNN)
A Convolutional Neural Network (CNN) is a type of Deep Learning neural network architecture commonly used in Computer Vision. Computer vision is a field of Artificial Intelligence that enables a computer to understand and interpret the image or visual data

Here are just a few popular computer vision applications where CNNs are used:

Facial recognition systems
Analyzing and parsing through documents
Smart cities (traffic cameras, for example)
Recommendation systems, among other use cases

The complete training process of a neural network involves two steps.

**1. Forward Propagation**

Images are fed into the input layer in the form of numbers. These numerical values denote the intensity of pixels in the image. The neurons in the hidden layers apply a few mathematical operations on these values
![Screenshot 2023-09-14 133045](https://github.com/vidhathri30/L1Report/assets/101579638/56478acd-2082-4f8c-b955-0160a63c4873)

Forward Propagation Summary
Step 1: Load the input images in a variable (say X)

Step 2: Define (randomly initialize) a filter matrix. Images are convolved with the filter

Z1 = X * f
Step 3: Apply the Sigmoid activation function on the result

A = sigmoid(Z1)
Step 4: Define (randomly initialize) weight and bias matrix. Apply linear transformation on the values

Z2 = WT.A + b
Step 5: Apply the Sigmoid function on the data. This will be the final output

O = sigmoid(Z2)


**2. Backward Propagation**

Once the output is generated, the next step is to compare the output with the actual value. Based on the final output, and how close or far this is from the actual value (error), the values of the parameters are updated. The forward propagation process is repeated using the updated parameter values and new outputs are generated.

![Screenshot 2023-09-14 133143](https://github.com/vidhathri30/L1Report/assets/101579638/535d29a2-7dad-4dda-8838-4d08030655d5)


1. Change in Z2 with respect to A1
To find the value for ∂Z2/∂A1 , we need to have the equation for Z2 in terms of A1:

Z2 = WT.A1 + b
On differentiating the above equation with respect to A1, we get WT as the result:

 ∂Z2/∂A1  = WT
 

2. Change in A1 with respect to Z1
The next value that we need to determine is ∂A1/∂Z1. Have a look at the equation of A1

A1 = sigmoid(Z1)
This is simply the Sigmoid function. The derivative of Sigmoid would be:

 ∂A1/∂Z1 = (A1)(1-A1)
 

3. Change in Z1 with respect to filter f
Finally, we need the value for ∂Z1/∂f. Here’s the equation for Z1

Z1 = X * f
Differentiating Z with respect to X will simply give us X:

∂Z1/∂f = X

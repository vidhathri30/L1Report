

## Task1

## Linear Regression:
Linear Regression is a machine learning algorithm that determines the relationship between one dependent variable (y) and one or more independent variables (x). It models a target prediction value based on the dependent variable, using this determined relationship. 

A linear regression line has the equation **Y=mX + b**

where Y is the dependent variable, m is the slope, X is the dependent variable and b is the y intercept. 

If there is more than one independent variable, the equation will be modified to 

**Y = m<sub>1</sub>X<sub></sub>1</sub> +</sub> m<sub>2</sub>X<sub>2</sub> + m<sub>3</sub>X<sub>3</sub> + … + b**

 **NumPy** supports large multi-dimensional arrays and matrices, along with a large collection of mathematical functions to operate on these.
 
**Pandas** a software library written mainly for data manipulation and analysis purposes.

  **Scikit-learn** is a popular machine learning library with various classification, regression and clustering algorithms.
  
**Matplotlib** is a library that works as an extension of NumPy. It provides an API for embedding plots into applications.

The steps involved in implementing the model are as follows:

1.  Initially the libraries are imported

    
    ![task11](https://user-images.githubusercontent.com/116189666/227711961-217a5166-d013-488f-8851-2c75876959ed.jpg)

 2.  The California housing  price data is loaded from the datasets. The target contains the prices of the houses feature_names contain the names of all the features in the dataset (except target variables). Before moving on to the next step, the data is checked for any missing values i.e the null values. There are no missing values in the dataset

     ![Screenshot 2023-09-13 231015](https://github.com/vidhathri30/L1Report/assets/101579638/7c4e3439-c79a-4778-8c8f-a0973bbb4886)
     ![Screenshot 2023-09-13 231416](https://github.com/vidhathri30/L1Report/assets/101579638/d5374099-685c-4ce4-9228-12e2034a6421)

 4.  The data splitted as training data and testing data The size value 0.1 indicates that 90% of the samples are used to train the model and the remaining 10% to evaluate or test the model. For this purpose, we use we utilize the scikit learn library's train_test_split() function as shown

![Screenshot 2023-09-13 232954](https://github.com/vidhathri30/L1Report/assets/101579638/27efe748-1b64-4c1d-9769-5eac114ebc2a)

 5.  Scikit learn's LinearRegression() is used to train our model on both the training and test sets

![task14](https://user-images.githubusercontent.com/116189666/227711986-595c63b1-dc57-4316-a648-07b9b9fededf.jpg)

 5.  This step is to determine whether the model is overfitting or not. Overfitted models perform well on test datasets but do not predict well on real-world datasets The root mean squared error(rms) and R2 score is used to assess the overfitting. The R2 score is of both training and testing data are almost equal to one. Hence the model is not overfitting.

![Screenshot 2023-09-13 233010](https://github.com/vidhathri30/L1Report/assets/101579638/bab81274-22c0-4098-8c26-44b124047164)

6.Finally the actual prices vs predicted prices are visualized using scatter plot

![Screenshot 2023-09-13 233048](https://github.com/vidhathri30/L1Report/assets/101579638/3fdefc3a-1c5c-4caf-8bbd-d7afde123794)



## Logistic Regression -
Logistic Regression is a classification algorithm. It models the probability of an event taking place by plotting the logarithmic sigmoid (to bring the output between 0 and 1) of a linear combination of independent variables. 

Concepts like maximum likelihood and the decision boundary are used in this model to classify the given data into required categories.

Something to note is that classification requires probability of the class and therefore should be between 0 and 1, in contrast to linear regression which places no bounds on the predicted outcome.

Here, we pick up the iris dataset containing 50 instances each for three species of flowers (Iris Setosa, Iris Versicolor and Iris Virginica) and their four attributes - petal width and length and sepal width and length. 

The modules and libraries used are the same as the ones in linear regression except for one - **Seaborn**, a data visualization library based on matplotlib. It is used mainly for integrating high-level statistical graphics.

The implementation of the model can be split up into the following steps:

 1.Importing all the dependent modules and libraries

![Screenshot 2023-09-14 000252](https://github.com/vidhathri30/L1Report/assets/101579638/8571f274-b3d5-4ebd-8999-05b81a88608c)

 2. load the iris dataset into a local variable

![Screenshot 2023-09-14 000330](https://github.com/vidhathri30/L1Report/assets/101579638/e9393dce-9fc8-4f84-a869-546aa2b38083)


Note that here, data refers to the x values, target refers to the y values and feature names refer to the column names.
    
 
3. Viewing the first 5 rows of the created DataFrames

   ![Screenshot 2023-09-14 000409](https://github.com/vidhathri30/L1Report/assets/101579638/0d7bf430-ee90-4b70-aeac-ed40ef7cf7f1)
   
 
 4. we create an instance of sci-kit’s logistic regression model and then go on to split the data into training and testing sets

  ![Screenshot 2023-09-14 000502](https://github.com/vidhathri30/L1Report/assets/101579638/09acaaff-b575-4032-ad10-b164926329f8)

 5. we ‘fit’ the model using the training sets we just created.

 ![Screenshot 2023-09-14 001002](https://github.com/vidhathri30/L1Report/assets/101579638/f2ad80a2-3f95-4db5-a1f7-11312ad2e00b)

  6.Viewing the coefficients and intercepts of the linear relationship the model has arrived at
  
![Screenshot 2023-09-14 001048](https://github.com/vidhathri30/L1Report/assets/101579638/c9cc4b8a-b35a-4678-9a02-9216f054fe60)

  7.Now, we use the relationship determined by the model to predict y values for the testing set

  ![Screenshot 2023-09-14 001103](https://github.com/vidhathri30/L1Report/assets/101579638/c2dae474-bf48-4e70-b4cd-719d4eb0185c)
  
  8.We plot the confusion matrix for the data and the corresponding predictions

  ![Screenshot 2023-09-14 001113](https://github.com/vidhathri30/L1Report/assets/101579638/0b517901-5cff-4667-8f6a-1965427a3238)
 
 A confusion matrix is a performance measurement for machine learning classification. So here, the numbers along the diagonal of the matrix (16,10,11) are all the times our model was accurate while the other numbers point out the times our model messed up.
 This matrix can be viewed better with the help of Python’s seaborn library which is what we do next
  
  
 9. we use one of the default metrics (score) offered by sklearn to calculate the accuracy of our model.

 ![Screenshot 2023-09-14 001125](https://github.com/vidhathri30/L1Report/assets/101579638/45ed1489-6f76-43cf-b403-96cda62fbe24)
 
  Hence, our model is 100% accurate


     
    

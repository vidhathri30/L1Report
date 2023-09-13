

## Task1

The data is imported as a pandas dataframe, then we add the house prices to it. This will allow us to manipulate this data mathematically by using inbuilt methods in pandas which is called data cleaning.

We will start with importing basic modules such as numpy, pandas and matplotlib. We put the data into a data frame which behaves like an 2D array in C, using Pandas. With data frames we can manipulate the data mathematically by using inbuilt methods in pandas which is called data cleaning.

We will use a set of data that helps us understand the relationship between variables. We import numpy to convert the data from Pandas into a 2D array. Then we can manipulate the data mathematically by adding columns and slicing it in different ways with pd.DataFrame().

Linear Regression is a supervised learning algorithm, which means that it works on a set of labeled examples. Before we look at how to use linear regression in Python, let's first learn about the concepts we need to understand before using the appropriate methods,

The steps involved in implementing the model are as follows:

1.  Initially the libraries are imported

    
    ![task11](https://user-images.githubusercontent.com/116189666/227711961-217a5166-d013-488f-8851-2c75876959ed.jpg)

 2.  The California housing  price data is loaded from the datasets. The target contains the prices of the houses feature_names contain the names of all the features in the dataset (except target variables). Before moving on to the next step, the data is checked for any missing values i.e the null values. There are no missing values in the dataset

     ![Screenshot 2023-09-13 231015](https://github.com/vidhathri30/L1Report/assets/101579638/7c4e3439-c79a-4778-8c8f-a0973bbb4886)
     ![Screenshot 2023-09-13 231416](https://github.com/vidhathri30/L1Report/assets/101579638/d5374099-685c-4ce4-9228-12e2034a6421)

 4.  The data splitted as training data and testing data The size value 0.2 indicates that 80% of the samples are used to train the model and the remaining 20% to evaluate or test the model. For this purpose, we use we utilize the scikit learn library's train_test_split() function as shown

![Screenshot 2023-09-13 232954](https://github.com/vidhathri30/L1Report/assets/101579638/27efe748-1b64-4c1d-9769-5eac114ebc2a)

 5.  Scikit learn's LinearRegression() is used to train our model on both the training and test sets

![task14](https://user-images.githubusercontent.com/116189666/227711986-595c63b1-dc57-4316-a648-07b9b9fededf.jpg)

 5.  This step is to determine whether the model is overfitting or not. Overfitted models perform well on test datasets but do not predict well on real-world datasets The root mean squared error(rms) and R2 score is used to assess the overfitting. The R2 score is of both training and testing data are almost equal to one. Hence the model is not overfitting.

![Screenshot 2023-09-13 233010](https://github.com/vidhathri30/L1Report/assets/101579638/bab81274-22c0-4098-8c26-44b124047164)

6.Finally the actual prices vs predicted prices are visualized using scatter plot

![Screenshot 2023-09-13 233048](https://github.com/vidhathri30/L1Report/assets/101579638/3fdefc3a-1c5c-4caf-8bbd-d7afde123794)


     
    

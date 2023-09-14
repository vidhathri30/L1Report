# Linear and Logistic Regression - Coding the model from SCRATCH
## Linear Regression
As we already know, linear regression is a machine learning algorithm that determines the relationship between independent and dependent variables. It models a target prediction value determined from this relationship. There are two main concepts involved in implementing this - cost function, gradient descent.


Linear Regression  
![t41](https://user-images.githubusercontent.com/116189666/227723615-282c6dee-2e2a-439a-81d3-939e51bd6411.jpg)

Implementation of linear regression model on a particular dataset involves various functions. The key concepts involved in deriving the linear regression model are as follows
Given our simple linear equation y=mx+b, we can calculate MSE as:  
![t42](https://user-images.githubusercontent.com/116189666/227723620-27520b7a-67a5-4630-919a-fc4edda99626.jpg)

 
We can calculate the gradient of this cost function as:
 
The steps involving in implementation of the linear regression model are as follows:
1.	Firstly we create a class LinearRegression. In the init function we set the learning the rate value to 0.001 and number of iterations to default value 1000  
 ![t43](https://user-images.githubusercontent.com/116189666/227723627-fa479792-7b0e-488c-95b7-d25d52fc134d.jpg)

2.	Now we define a fit method which takes the training samples and labels associated with them and the gradient descent function is implemented in this step as per the formula specified  
 ![t44](https://user-images.githubusercontent.com/116189666/227723635-62799abb-2cbb-465e-99d3-9820774cfe50.jpg)

3.	Then the predict method is defined which gets the new test samples  
 ![t45](https://user-images.githubusercontent.com/116189666/227723639-ac7873bc-8a04-43f4-946a-60fa391029cf.jpg)

4.	The necessary libraries are imported  
 ![t46](https://user-images.githubusercontent.com/116189666/227723659-8e809269-04a2-442a-b656-5244a8bdf5f6.jpg)


5.	The data splitted as training data and testing data The size value 0.2 indicates that 80% of the samples are used to train the model and the remaining 20% to evaluate or test the model. For this purpose, we use we utilize the scikit learn library's train_test_split() function as shown

 ![t47](https://user-images.githubusercontent.com/116189666/227723664-d938847a-7ded-408f-839e-a9f9457e9ada.jpg)

6.	The training data and testing data are fit into the dataframe and the test values are predicted

7.	The cost function is defined as mse to calculate the mean squared error and the accuracy of the model is calculated
 ![t48](https://user-images.githubusercontent.com/116189666/227723669-efcbbf9b-1807-40c0-9a74-c76364ee4534.jpg)

8.	The scatter plot is used to visualize the data which has been approximated

![Screenshot 2023-09-14 125320](https://github.com/vidhathri30/L1Report/assets/101579638/8dce5930-6c9a-4fc5-861a-a2640f2aaa1d)

## Logistic Regression
Unlike linear regression, logistic regression works using the sigmoid function to return a probability curve using the sigmoid function. This logistic function returns a probability value which then leads to either one of two discrete classes. The sigmoid function keeps all values between 0 and 1 and is given by the equation

![10](https://user-images.githubusercontent.com/116189666/227724687-91433bb1-e84b-4e47-b18b-f580832f474b.png)  

![11](https://user-images.githubusercontent.com/116189666/227724847-8d0b1087-35f4-43b0-bf64-5828fc5f09ee.png)

The steps involving in implementation of the logistic regression model are as follows:  



1.Firstly we create a class LogisticRegression. In the init function we set the learning the rate value to 0.001 and number of iterations to default value 1000
![12](https://user-images.githubusercontent.com/116189666/227724760-3e8f3971-1067-4736-ba32-c8391bd069f0.png)


2.Now we define a fit method which takes the training samples and labels associated with them and the gradient descent function is implemented in this step as per the formula specified

![13](https://user-images.githubusercontent.com/116189666/227724768-eda3cfad-6776-4422-b752-fb7816b53522.png)

3.Then the sigmoid function is defined as per the formula specified  

![14](https://user-images.githubusercontent.com/116189666/227724772-8a1e775d-bfab-4d18-adcb-b662b18cf46e.png)


4.Then the predict method is defined which gets the new test samples and approximate the values as per a linear model and uses sigmoid function. It predicts 1 if the value is greater than 0.5 and 0 if the value is less than 0.5


5.The necessary libraries are imported and the iris dataset is loaded

![16](https://user-images.githubusercontent.com/116189666/227724777-86fd3d3b-a679-415f-aaa4-454f8d774640.png)

6.The data splitted as training data and testing data
The size value 0.2 indicates that 80% of the samples are used to train the model and the remaining 20% to evaluate or test the model. For this purpose, we use we utilize the scikit learn library's train_test_split() function as shown


![17](https://user-images.githubusercontent.com/116189666/227724784-7fe1858c-656f-4511-b31f-c5cd3ad4a3a0.png)

7.The training data and testing data are fit into the dataframe and the test values are predicted
![18](https://user-images.githubusercontent.com/116189666/227724785-9631eda1-52cb-4c56-a671-45ad258784da.png)


8.Lastly the accuracy function is used to obtain the accuracy of the model
![19](https://user-images.githubusercontent.com/116189666/227724786-fa6948d0-b482-4cb1-b1fe-8f09c5c8c25c.png)


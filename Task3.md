## Task 3: Metrics and Performance Evaluation

The most important aspect of building models is finding its accuracy on training data using the **right** metrics. Choosing the right metric based on our need for the model and its results is very important so that we can optimize and fine tune the model’s performance as needed. 

**1. Regression Metrics - used to evaluate performance of regression algorithms**

  The regression model predicts continuous target values. These are different from the classification metrics because they should be able to work on continuous values.

**Mean Absolute Error(MAE)**

  The regression model predicts continuous target values. These are different from the classification metrics because they should be able to work on continuous values.

![Screenshot 2023-09-14 120759](https://github.com/vidhathri30/L1Report/assets/101579638/44fba74d-77eb-494c-a6ea-1c7d5f56877c)
![Screenshot 2023-09-14 120521](https://github.com/vidhathri30/L1Report/assets/101579638/519747c1-4621-4d03-9260-c98a2c276da3)



**Mean Squared Error(MSE)**

This essentially finds the average squared error between the predicted and target values. It shows the deviation in the values. Outliers have a larger effect on this metric because we’re squaring the distance. If yi is the true value and y^i is the corresponding predicted value, then MSE is given as:


![Screenshot 2023-09-14 120811](https://github.com/vidhathri30/L1Report/assets/101579638/f225342a-40c2-4c9b-8797-3f83996d2718)
![Screenshot 2023-09-14 120857](https://github.com/vidhathri30/L1Report/assets/101579638/b90d967a-3cbd-4d6e-b370-37baa88ef879)

**Root Mean Squared Error(RMSE)**

 RMSE which is just the root of the Mean Squared Error. This handles penalization of smaller errors by taking the square root. The formula is given by:

![Screenshot 2023-09-14 120819](https://github.com/vidhathri30/L1Report/assets/101579638/2d83a132-772a-482b-9b5d-638a0eec20a3)
![Screenshot 2023-09-14 120910](https://github.com/vidhathri30/L1Report/assets/101579638/58b699f0-837f-4dc5-aadb-c73267c39a11)

**R Squared (R2)**

This is a post metric i.e., a metric that is calculated using other metrics. It essentially is just a measure of what percentage of the total variation in target is explained by the regression line we plot. Closer this value is to 1, the better our model’s accuracy is.

![Screenshot 2023-09-14 120833](https://github.com/vidhathri30/L1Report/assets/101579638/cd122b9d-797b-4c43-b82b-5d10e1b2092f)
![Screenshot 2023-09-14 120920](https://github.com/vidhathri30/L1Report/assets/101579638/9d712162-914f-407b-b5b0-55ee1a64bdb4)


**Adjusted R Squared**

The disadvantage of the R2 score is while adding new features in data the R2 score starts increasing or remains constant but it never decreases because It assumes that while adding more data variance of data increases.

![Screenshot 2023-09-14 121600](https://github.com/vidhathri30/L1Report/assets/101579638/5424a3ae-2d1b-467f-9dc4-9437e4c5540f)


**2. Classification Metrics - used to evaluate performance of classification algorithms**

 Classification is one of the widely used models in Machine Learning. It mainly involves predicting classes depending on the input we have. Binary classification is the type of classification where only two classes are involved. A decision boundary is set and any value above this points to a certain class while any value below points to another value. 

 **Classification Accuracy**
 
    This is the simplest metric which just takes the ratio of number of correct predictions to total number of predictions. This is analogous to the accuracy_score() function.

    ![Screenshot 2023-09-14 122832](https://github.com/vidhathri30/L1Report/assets/101579638/e71119b5-3958-4d59-9daa-1f0df62d1695)


 **Confusion Matrix**
 
  This is a function that computes the confusion matrix with each row corresponding to the true class. So it essentially is a matrix of true and false positives and negatives. Within a confusion matrix, we have multiple metrics like precision, recall and F1 score.

![Screenshot 2023-09-14 122907](https://github.com/vidhathri30/L1Report/assets/101579638/e6e5d8a6-6aeb-4c35-bab5-261def1d1393)

  **Classification Report**
  
    This conveniently builds a report with results of all the main classification labels.

    ![Screenshot 2023-09-14 122948](https://github.com/vidhathri30/L1Report/assets/101579638/c8188fff-222f-4153-a7b4-a12184459efe)





















    \

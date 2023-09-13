**Implement KNN using sci-kit’s neighbors.KNeighborsClassifier for multiple suitable dataset
The steps involved in implementing scikit learn library are as follows:**  
1.	Initially the libraries required are imported
 ![t51](https://user-images.githubusercontent.com/116189666/227725589-e259fcd7-1bfa-4207-8cc9-c6bf58c3958a.jpg)

2.	The iris dataset is loaded from the Iris.csv file stored in the location
 ![t52](https://user-images.githubusercontent.com/116189666/227725596-2e7a5631-4560-4ac3-87ea-4b60b1b43bd8.jpg)

3.	All the features and their values can be displayed as shown
 ![t53](https://user-images.githubusercontent.com/116189666/227725600-7b922fd0-b920-4564-9044-d86a17405bf1.jpg)

4.	Since the species has many null values it cannot be considered for training and testing. Hence except that column and its values the rest are considered and stored in x
 ![t54](https://user-images.githubusercontent.com/116189666/227725623-d113a4f7-143c-4fce-a1f2-8229833d6dc3.jpg)

5.	The species column with names are considered and stored in y
 ![t55](https://user-images.githubusercontent.com/116189666/227725637-feba197d-3616-40c2-8b49-58534eeb4c75.jpg)

6.	To locate the data point in multidimensional feature space, it would be helpful if all features are on the same scale. Hence normalization or standardization of data will help
 ![t56](https://user-images.githubusercontent.com/116189666/227725644-4fbb7c99-4a90-4447-9e3a-6d2f1c4d5de2.jpg)

7.	The data splitted as training data and testing data The size value 0.3 indicates that 70% of the samples are used to train the model and the remaining 30% to evaluate or test the model. For this purpose, we use we utilize the scikit learn library's train_test_split() function as shown
 ![t57](https://user-images.githubusercontent.com/116189666/227725664-1885bea7-1d09-4ad3-ab55-f6a9c48bc9ac.jpg)

8.	The accuracy function is used to calculate the accuracy of the model
 ![t58](https://user-images.githubusercontent.com/116189666/227725678-722caa40-72ca-43f3-a939-b2f5ae21d08d.jpg)

9.	The confusion matrix is imported from the library and gives us an idea about which of the values are not classified properly
 ![t59](https://user-images.githubusercontent.com/116189666/227725692-86203fd6-706f-4c53-a0d8-ff21f313bfe8.jpg)

__Implement KNN from scratch. Compare results with sci-kit’s built in method for different datasets.
Implementation of KNN algorithm from scratch involves the following steps:__
1.	The euclidean_distance function is defined which computes the distances from a specific as described in the formula
 ![t510](https://user-images.githubusercontent.com/116189666/227725698-6991db7e-e573-46d9-9510-2573f8da7412.jpg)

2.	The KNN class is defined. It consists of fit, predict and _predict method. The fit method stores the training samples. The predict method stores multiple samples of data whereas the _predict method takes only one data sample. _predict method computes the distances and gets the k nearest samples and also the most common class label.
 ![t511](https://user-images.githubusercontent.com/116189666/227725710-8738bb8a-884c-45ce-9e01-55c549c4cc51.jpg)

3.	The necessary libraries are imported which are required for the implementation of the model and the iris dataset is loaded from the datasets. X and y have the data values and target values respectively
 ![t512](https://user-images.githubusercontent.com/116189666/227725720-56fdcb74-6d3c-41c7-a7a0-bce4eaa773c4.jpg)


4.	The data splitted as training data and testing data The size value 0.2 indicates that 80% of the samples are used to train the model and the remaining 20% to evaluate or test the model. For this purpose, we use we utilize the scikit learn library's train_test_split() function as shown
  ![t513](https://user-images.githubusercontent.com/116189666/227725741-30ee8bf0-241c-4485-a92a-1da1e3f3f91e.jpg)

5.	The data is then fit into the data frame and the accuracy is calculated
 ![t514](https://user-images.githubusercontent.com/116189666/227725748-34960ff8-d826-4792-8695-f18b3420234e.jpg)

When compared both the models are returning approximately the same value

Conclusion:
The k-NN algorithm is a simple and effective algorithm that can be used for both classification and regression problems. Its performance depends on the choice of k and the distance metric used. In practice, the k-NN algorithm is often used in combination with other algorithms for improved performance

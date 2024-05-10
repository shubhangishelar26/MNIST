# MNIST handwritten digit recognition 
Problem Statement:
Take the standard MNIST handwritten digit dataset, and as usual, split it into training and testing data. Treat each image as a vector. For all the test images, calculate the nearest neighbor from the training data, and report this label as the prediction. 

#Steps


1.	Load Data: Load the MNIST dataset and split it into training and testing sets.
2.	Visualize Data: Optionally, visualize a few sample digits from the training set.
3.	Split Training Data: Further split the training data into training and validation sets.
4.	Train and Validate: Train a k-Nearest Neighbor classifier with different values of k, and evaluate each model's accuracy on the validation set.
5.	Select Best Model: Determine the k value that achieves the highest accuracy on the validation set.
6.	Final Training: Retrain the classifier using the best k value.
7.	Predict and Evaluate: Predict labels for the test data using the trained classifier and calculate the accuracy.
8.	Report Results: Print the accuracy score and any other relevant evaluation metrics.





================================Questions==============================================

1.How accurate is this method?
---->98% on an average


2.What metric did you use for distance?
----> Default Euclidean distance metric.

3.How fast/slow is your implementation? Can you analyze the bottlenecks and speed things up?
---->mplementation speed depends on dataset size and k value. Bottlenecks may arise from high dimensionality. Efficient algorithms and data structures in scikit-learn help mitigate this.

4.Any ideas on improving accuracy?
---->Consider feature scaling, dimensionality reduction (like PCA), optimizing hyperparameters, or using ensemble methods.


# Decision Trees -> Regression Tree

A regression tree automatically selects important predictors and suggests trading rules. The predictor variables are one-day returns, five-day returns, five-day standard deviation and so on. The target variable is one-day future return. 
<BR>

<B>Create a regression tree</B>
1. Import stock data
1. Define predictor variables and a target variable
2. Split the data into train and test 
3. Create a regression tree model using the training data
4. Visualize the model

<B>Analyzing the performance</B><BR><BR>
Part I: Single leaf
1. Trading rule based on one leaf node with the highest expected value of a target variable
5. Compute performance in the train and test dataset

Part II: Full tree
1. Trading rule based on all the leaf node
5. Compute the performance in the train and test dataset
![image](https://user-images.githubusercontent.com/52425750/165808566-7462b4fb-7395-4af9-995d-b0f26f22e30e.png)

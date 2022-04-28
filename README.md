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


 ## Data Source
Historical data was collected from the Yahoo finance library. The data starts from January 1st, 2009 and up till April 25, 2022. The yahoo finance library is very simple and easy to use. The data collected were the daily prices of the stocks, the high, low, open, close, adj close and volume.
 ### Apple Stock Closing Price
![image](https://user-images.githubusercontent.com/52425750/165809695-07dffdd7-44b3-4b11-9fa2-07e286d8d9ab.png)
  ## Modeling 
The model used to predict future returns is the regression tree model. There are two strategies involved:
  1. Single Leaf -> Buy when the value of the ATR indicator is greater than .326 and the 5-day standard deviation is greater than .01
  2. Full Tree -> Buy if the expected value is positive or else sell the stock
  
![image](https://user-images.githubusercontent.com/52425750/165811719-2dab44ae-ae3b-464c-9939-57bbbf854228.png)
 ## Strategy Results
 ![image](https://user-images.githubusercontent.com/52425750/165812625-d898c79b-7d22-4448-a20c-5e5682f80253.png)
## Visualizing Entry and Exit Points
 ![image](https://user-images.githubusercontent.com/52425750/165812721-9199628c-bdbc-400a-b96a-29b26fbb3ac0.png)
## Pyfolio Backtest
 ![image](https://user-images.githubusercontent.com/52425750/165813101-2b3a3d28-3669-4718-9857-f2dfdb887b3e.png)
 ![image](https://user-images.githubusercontent.com/52425750/165813123-a2b237f8-6b66-4d32-896a-e4823237bb9c.png)



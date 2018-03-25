# Linear-Regression-With-Multiple-Variable

You are selling your house and you want to know what a good market price would be. 

Predict the price of a house with 1650 square feet and 3 bedrooms

----------- input ----------- <br>
ex1data2.txt contains a training set of housing prices in Port- land, Oregon. 
The first column is the size of the house (in square feet), the second column is the number of bedrooms, and the third column is the price of the house.

α = 0.01;<br>
num_iters = 400;

Given predict the price of a house with 1650 square feet and 3 bedrooms ?


<b>How to Solve this ?</b><br>

<img src="Linear%20Regression%20-%20Multiple.png">

<b>Step 1:</b> Normalize the data, i.e  normalized_value = current_value * mean / standard-deviation

<b>Step 2:</b>  Based on formula, calculate theta:
  
  theta = theta - (alpha / m) * (X'*X*theta - X' * y);
  
<b>Step 3:</b> Predict for some value house with 1650 square feet and 3 bedrooms ?
  
  normalize_size =  1650 - mean(sq.ft) / std(sq.ft)
  normalize_rooms = 3 - mean(rooms) / std(rooms)
  
  Y = [ 1 , normalize_size,  normalize_rooms] * theta

  
 Reference: 
 http://openclassroom.stanford.edu/MainFolder/DocumentPage.php?course=MachineLearning&doc=exercises/ex3/ex3.html
 https://www.coursera.org/learn/machine-learning

# Predicting the next items in a grocery ordering & delivering app:<br> <br> Instacart Market Basket Analysis

Roberto Andrade Martínez

### Summary
<br>

Given Instacart's open source dataset, [3 million Instacart Orders](https://www.kaggle.com/competitions/instacart-market-basket-analysis/data), in which there is information of millions of sales transactions that have been made through the app, it is of interest to try to determine if there are certain hidden patterns regarding consumer decisiones within the data. 
<br><br>
Instacart itself asked some of this questions, like when would a user try a product for a first time, or if the user would buy one product for a second time.
<br><br>
The interesting aspect about Instacart's challenge is that they arranged their transactions data into two files, one for training and one for testing: they intended to use a supervised ML model to answer those questions.
<br><br>
The purpose of this project is to answer at least one of the questions: Which item will the user add to the basket next?, but with a slightly different approach, by using an unsupervised ML model.
<br>
<br>
To answer this question we will use the [apriori algorithm](https://www.vldb.org/conf/1994/P487.PDF), a classic ML model for association rules, and will implement it using the Python library [MLextend](https://rasbt.github.io/mlxtend/api_subpackages/mlxtend.frequent_patterns/), in particular the frequent_patterns subpackage. We are expecting to deliver a set of rules in which we indicate a given product that the user would add to the basket and then a consequent item which would be more likely to be added given what is already in the bag.
<br>
<br>
Implementing this algorithm in the application will surely increase customer retention and transactions as the overall experience will be enhanced and users will find it easier and faster to do their shopping in this app compared to the competition.
# Predicting bundles in a bakery

Roberto Andrade Martínez

### Summary
<br>
After observing and collecting sales data from a local bakery for almost six months, plenty of questions regarding the shop's performance come to mind, such as which products were the most popular, if certain products were sold more on certain conditions (such as a special day of the week), among others.
<br><br>
One such question, which this project intends to answer, is whether or not one product's sale is associated with that of another. In other words, if a product's chances of being sold are significantly higher when sold alongside another product rather than by itself.
<br>
<br>

To answer this question we will use the [apriori algorithm](https://www.vldb.org/conf/1994/P487.PDF), a classic ML model for association rules, and will implement it using the Python library [MLextend](https://rasbt.github.io/mlxtend/api_subpackages/mlxtend.frequent_patterns/), in particular the frequent_patterns subpackage.
<br><br>
The objective is to get a list of rules in which we indicate products that are antecedents and consequents of on another. Given this information, we could expect the bakery to act on it and potentially place some of this bundles together and plan its discount accordingly, so that it may increase revenue on those products and overall.
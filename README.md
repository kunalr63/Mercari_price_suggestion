# Mercari_price_suggestion
#INTRODUCTION:
It is said that data is the new oil , it means that collecting data would generate as much revenue as oil did over the past few centuries. Now , data in its raw form is not very useful just like oil and needs to go through some refining which would increase its usefulness in multiple areas .One such area is that of machine learning which is using the data we collected to make the machines learn from that data and based on that learning use it work on future data. Now in this case study I will solve a kaggle problem using the concepts of machine learning.

#BUSINESS PROBLEM:
The problem is a kaggle competition conducted by a Japanese company named Mercari . Mercari is a platform where people sell their products which are mostly used products so when a seller wants to sell his product on the website he/she would not always be sure as to how much the product should be sold for and this brings us to the problem at hand which is to suggest appropriate price to the seller for his product. Suggesting an appropriate price also affects the business because if the price suggested is too low then the seller might lose interest in selling the product on the platform and if the price suggested is too high then it will be difficult to find a buyer for it. Thus price suggested should be between the two boundaries.

In this problem the sellers inputs data about product like name , category , condition , shipping and description and based on them we have to suggest an appropriate price but this is not an easy task because price of product depends on very small details like in case of clothing it will depend on material , brand, colour and so on. Two product could have the almost similar details but price may differ drastically. For example the “Vince long-sleeve turtleneck pullover,Black,Women’s,Size L,great condition” and “St. John’s long-sleeve turtleneck pullover,Women’s,Size L,great condition” have similar data but their prices are very different.

#MACHINE LEARNING PROBLEM:
Since Price , the target variable is continuous thus its a regression problem . For each item the features available are id,name of the item,condition of the item,category,description and price.

We will divide the training data into train and cross validate. After training the model we would test it on the test data which the model has never seen.
BUSINESS CONSTRAINTS :

Mercari mentioned in the challenge that training and testing time should not be more than 60 mins on 16 GB RAM CPU thus it can be assumed that model should not take hours to run. If a sellers inputs all the required data about the product he should not be made to wait for hours before a price is suggested thus latency matters.

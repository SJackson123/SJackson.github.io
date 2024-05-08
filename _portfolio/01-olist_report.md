---
title: "Olist Power BI Report"
excerpt: "Power BI report on Olist E-Commerce Reviews.<br/><center><img src='https://github.com/SJackson123/SJackson.github.io/blob/master/images/olist/scr1.png?raw=true?raw=true' width='640px'></center>"
collection: portfolio
---
In this project, I make a Power BI report on feedback from Olist reviews with drill down fields and tool tips.

## Who is Olist?
Olist is an E-commerce company that connects small and micro businesses to retailers like Walmart for selling their products. Founded in 2014, I have access to data from 2016 to 2018 and draw out insights from the dataset found on kaggle. 

# How do ratings affect sales over time?
First, I created a dashboard on Feedback from reviews. In the top right of the report below, the average review score trend fluctuates at the end of 2016 and stabilises around an average of 4.1 from January 2017 onwards. 
<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/olist/scr1.png?raw=true?raw=true" alt="normalised histogram" width="640px"/>
</p>

In 2016 Olist did not perform well, with only 325 reviews and an average rating of 3.6. In December 2016, Olist only sold 1 product.

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/olist/dec2016.png?raw=true?raw=true" alt="normalised histogram" width="640px"/>
</p>

Sales in 2017 and 2018 contribute to the majority of Olist sales. Olist’s highest rated products generate the most profit (56.2%), however, there is a substantial minority of 1 star rated products. This was because popular products suffered problems with delivery in Brazil and took a long time to deliver overseas. Olist may benefit from adopting a flexible delivery scheme where self-employed delivery drivers can also deliver packages. This would create another way to get products quickly to customers and decrease the dependency on the main delivery channels.

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/olist/totalprofit.png?raw=true?raw=true" alt="normalised histogram" width="640px"/>
</p>

# What categories perform best over time?

The Cds and DvDs category had the highest rating but typically the highest rated product categories have very few reviews so an individual category does not contribute much to overall profit. This indicates Olist have a diverse range of products that are rated well, but do not contribute substantially to overall profit. Olist might benefit from streamlining their product range to focus on products with high ratings and high sales volumes.

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/olist/scr3.png?raw=true?raw=true" alt="normalised histogram" width="640px"/>
</p>

We can drill down into each product category and view the comments from reviews. Performing sentiment analysis and classifying feedback, we could identify the key problems in products.

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/olist/drilldown.png?raw=true?raw=true?raw=true" alt="normalised histogram" width="640px"/>
</p>

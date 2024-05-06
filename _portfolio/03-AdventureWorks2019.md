---
title: "AdventureWorks2019 Exploratory Data Analysis"
excerpt: "Combined SQL and Python to perform exploratory data analysis on the AdventureWorks2019 dataset."
collection: portfolio
---

Check out the repository <a href="https://github.com/SJackson123/AdventureWorks2019-Analysis">here</a>

During week 8 of my Data Analyst bootcamp at Generation, in groups of 4, we were tasked with completing a report on the database structure (ER diagrams and Schemas) and analysing the data to provide insights to six specific questions. This repository contains the code I developed to address three of those questions:

4. **What is the relationship between sick leave and Job Title (PersonType)?**
   -  Sales People (SP) are more likely to take less sick leave compared to other employees (EM)
6. **What is the relationship between store trading duration and Sales?**
   - No relationship between store trading duration and Sales
8. **What is the relationship between the size of the stores, number of employees and revenue?**
   - Strong positive relationship betweeen size of stores and employees - larger stores need more employees to run efficiently
   - No relationship between size of store or number of employees and revenue
   - Further analysis on additional predictors if AdventureWorks aims to increase revenue

## Q4) What is the relationship between sick leave and Job Title (PersonType)?

To start off, we define how we categories people. In the AdventureWorks2019 dataset, there are 6 categories of people:

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/AdventureWorks/PersonType.png?raw=true" alt="person_type" width="300px"/>
</p>

Only Sales Person (SP) and employees (EM) are elegible for sick leave hours. From the figure below, we see an almost uniform distribution of sick leave hours which tapers off after 70 hours.

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/AdventureWorks/histogram_hours.png?raw=true" alt="sick leave hours distribution" width="640px"/>
</p>

However, plotting the distribution of sick leave hours for each employee type tells a different story:

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/AdventureWorks/boxplot_persontype.png?raw=true" alt="normalised histogram" width="640px"/>
</p>

The box plot above compares the distribution of sick leave hours for EM and SP employees. Both distributions are relatively symmetric, with no outliers. This suggests the majority of sick leave hours fall within the interquartile range for both employee groups.

There is a noticeable difference when looking at the spread of sick leave hours between the two groups. EM employees have a wider spread of sick leave hours and a higher median of 46 hours, indicating that half of the EM employees take at least 46 hours of sick leave. ON the other hand, SP employees show a smaller spread in sick leave hours around a median value of 34.12 hours. This suggests that SP employees take fewer sickl leave hours compared to their EM counterparts.

These findings may indicate differences in sick leave policies between the two employee groups.

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/AdventureWorks/hist_separate_type.png?raw=true" alt="normalised histogram" width="640"/>
</p>

The histogram above illustrates the distribution of sick leave hours for two employee types: Employee non-sales (EM) and Sales person. The sick leave hours have been normalised to directly compare between the two groups.

Focusing on the histogram for EM employees, it has a nearly uniform distribution of sick leave hours with the range of 20 to 70 hours. The probability of an EM employee taking between 23 to 70 hours of sick leave is 93.04%, this demonstrates that a large proportion of EM emplyees tend to take sick leave within this range.

In contrast, the histogram for SP employees shows a more concentrated distribution of sick leave hours, with 94.12% of SP employees falling between 30 to 40 hours. This indicates that SP employees are more likely to take less sick leave hours compared to their EM employees. However, the sample size of SP employees is only 17, while there are 273 EM employees. The small sample size of SP employees limits the robustness of sick leave in this group.

Thank you for reading. You can find the analysis for Q5 and Q6  [here](https://github.com/SJackson123/AdventureWorks2019-Analysis/blob/main/Q5_analysis.ipynb) and [here](https://github.com/SJackson123/AdventureWorks2019-Analysis/blob/main/Q6_analysis_final.ipynb).



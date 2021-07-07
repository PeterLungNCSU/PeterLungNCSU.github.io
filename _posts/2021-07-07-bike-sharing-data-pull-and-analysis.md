---
layout: post
title: Bike Sharing Data Pull and Analysis
---


I just finished my part of the bike sharing data project. I say my part because it was a group project. I am going out of town this weekend when it's due, so I asked my partner, Caroline Baker, to publish it once it is complete.

It was a fun project. The data consisted of two years of UCI bicycle sharing data (2011 - 2012). They recorded the number of users as well as weather and temperature conditions for each day during the two year period. The goal of the project was to build a series of models to try and use the weather and seasonal data to predict the number of users. We had the option to use casual users, registered users, or the sum of the two and we chose the sum. We had to fit seven of these models, one for every day of the week.

# Project Description

We were each supposed to fit two models: one linear regression model and one tree model. My tree model was the boosted tree and Caroline did the random forest model. In pretty much every day of the week analysis, the random forest model won. There are a number of reasons for this, one is that linear regression models require a significant amount of TLC when it comes to getting a functional form that can compete with what a tree model can do automatically. The boosted tree model has an enormous amount of potential, but the runtime required to get the model into optimal form is prohibitive, so we kept the cross-validation and tuning parameter sizes on the smaller side (especially because we have to run seven of them).

We also did a good amount of exploratory analysis and generated tables and charts automatically based on the day of week. Caroline did the univariate analysis, including creating the histograms, and I generated the multivariate relationship graphs like scatterplots and line graphs. We each also generated some summary statistics and contingency tables.

At the end, we evaluated each model by RMSE and declared a winner for each day (Random Forest pretty much every time) in an automated fashion.

# Reflection

At the end of a project, it is often helpful to look back and evaluate how things went. Here are some thoughts about the project and what I might do if I were to repeat it:

## What would you do differently?

I would probably prefer to fit everything in a single model rather than have seven different models. The reduction in the data from fitting seven separate models makes the dataset size too small. Remember, there are only 731 observations when you include all seven days, so each day of the week ends up with barely over 100 observations, and then you have to split that into training and test sets!

## What was the most difficult part for you?

Whenever it comes to coding, it is easy to get stuck on some error that you can't figure out. This is what drives me bananas about these projects! I have spent 30 minutes trying to figure out why I am getting an error when it was just some dumb mistake that I made (and I should have known that's what was causing the error!)

## What are your big takeaways from this project?

Trees, trees, trees! People at my office are using boosted trees more and more often to fit their models, and for good reason - they forecast better in a lot of cases. One colleague mentioned that he is noticing that tree models are winning a large proportion of kaggle competitions recently. I am excited to start applying what I have learned about random forest, bagging and boosting to my models for work!

# Project links

Here is a link to the [github pages](https://cebaker3.github.io/ST558 Project2/) site.

Here is a link to the [github repo](https://github.com/cebaker3/ST558_Project2) site.



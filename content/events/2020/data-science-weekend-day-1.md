+++
title = "Data Science Weekend Day 1"
date = 2021-02-27
[taxonomies]
tags = []
+++

## [Data Science Weekend - Day 1](https://www.facebook.com/events/168027461419020)

<img src = "/2020/event-banners/dsw.jpg" height=20% width=50%> 

Facebook Event Link: [https://www.facebook.com/events/168027461419020](https://www.facebook.com/events/168027461419020)

Event Page: [dsatlse.github.io/DataScienceWeekend/](dsatlse.github.io/DataScienceWeekend/)

> Are you an enthusiastic junior who would like to explore the field of Data Science? Or are you a more intermediate learner looking to upskill and try your first datathon? Or maybe you'd just like to learn something new and meet like-minded people?

> LSESU Data Science Society is proud to announce its first flagship event: “Data Science Weekend - Navigating a Data-Centric World”.
Supported by the new LSE Data Science Institute, this 2-day event will include panel discussions by data scientists from the finance and consulting industries, beginner-friendly workshops and a 24-hour data science challenge open to all skill-levels.

> We welcome UK university students from all backgrounds, aiming to make this event Adaptable and Inclusive. Join us for a weekend of learning and professional growth you won't forget!


# Computational Social Science

+ Data Science is one of the most important human activities we need Democratised Data Science

+ Bridge between academia and non-academia, the private sector and beyond. 

+ Convergence between online education and university education

+ Interdisciplinary skills

+ Statistics is harder to learn. Parameter estimates vs prediction


# Life is not a Kaggle competition

Clients don't want "data reports" they want end products

+ EDA
+ Preprocessing
+ Modelling
+ Post preprocessing (clients are not data scientists, what do they want to see)


'virtual envs' - ensures reproducibility - https://docs.python.org/3/library/venv.html

`Streamlit` - allows building data apps

`pandas_profiling` - quick EDA

Data Mining from EDA vs getting questions / problems from clients

Real world  - data is missing for a reason, can't just drop NAs. 

Data preprocessing can help data more meaningful to clients

Types - `scikit-learn` is still unstable - what should it take in (Nans, floats, categories)

Not all models are statistical. Many deterministic solutions as opposed to statistical - Graph Theory for understanding networks, Linear Programming for optimisation. Problems are very sensitive to Hyperparameters - e.g. word2vec and domain problems

baseline models (Logistic Regression, Linear Regression) might not achieve convergence efficiently enough in a business setting / so Deep Learning and SGD might work better. `pytorch-lightning-bolts`

Understand your customer objectives, moving towards Bayesian framework - parameters in these confidence intervals under these assumptions as opposed to frequentist confidence intervals

1. Check your data types
2. Transform your data
3. Make sure your data is in the right type for your *models*
4. Models

+ http://www.stat.columbia.edu/~gelman/book/

+ https://github.com/topher-lo/streamlit-e2e-boilerplate

+ R Shiny `tidyverse`

# Consulting Panel


**In your opinion which industries are the most advanced in leveraging data science to create value, and where would you like to see more progress? Could you walk us through a common/ innovative application/use case?**

+ Retail - marketing analytics , lots of data on this (discounts)
+ Chatbots
+ Utilities - in part due to Internet of Things (IoT). Have lots of unstructured data
+ Public Sector 
+ Genomics - 

**What advice would you give to students looking to pursue a similar career path? Which skills do you think consulting firms look for in potential recruits?**

+ Passion (Side projects , Kaggle). Find out what part of data science interests you
+ Communication skills
+ Python, SQL
+ Model building frameworks, e.g. Pytorch (fast.ai), Tensorflow (Coursera)
+ Possibly Cloud
+ Problem solving abilities probably the most key, 


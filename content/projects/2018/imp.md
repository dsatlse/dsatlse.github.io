+++
title = "Industry Mentorship Programme"
date = 2018-06-22
[taxonomies]
tags = ["recsys", "pytorch"]
+++

# Amazon Recommender System

It started as the Industry Mentorship Programme with Datatonic.

## Quick recap
* We are using the Amazon reviews dataset book 5-core with approx. 9 million reviews
    * The dataset is available at [link](http://jmcauley.ucsd.edu/data/amazon/)
    * It is the largest dense subset available, the second largest one is 1.5M in size
    * Books have uniformal cover images, as opposed to e.g. Office Products or Pet Supplies
* We decided on using the Rendle's Factorization Machine
    * It's simple to understand and implement
    * It has linear runtime
    * There are potential extensions to online learning (more about this later)
* As an end product we want to develop and deploy a "sanity check" web application

## The "sanity check" web application
* The user is asked for full ratings of 5 books randomly chosen from the dataset
* We predict that user's rating for a large number of randomly chosen book from the dataset
* We show best 5 and worst 5 as the result
* We ask user for feedback about the chosen book which will become the main source of evaluation

## What we've done
* A preprocessing pipeline for a small subset of Books 5-core is available [here](https://gitlab.com/mlatlse/amazon-recsys)
* We've implemented 2nd order offline FM for sparse input with a ~0.9 RMSE in TensorFlow, [here](https://gitlab.com/mlatlse/amazon-fm)
* We've designed the "sanity check" application and drafted a RESTful API to plug into the model later on, [here](https://gitlab.com/mlatlse/amazon-app)

## Problems
* Write or find a package for sparse encoding for also_rated set categorical feature
* Online formulation: adding new users requires retraining the whole dataset

## Online formulation
* Since the FM whitepaper in 2010 there were some attempts to formulate convex FM, which would allow to use existing frameworks for online machine learning, namely the Online Convex Optimization framework (in vanilla FM the \hat{y} is non-convex with respect to the pairwise interactions vector (Blondel, 2015), (Yamada, 2017))
* We could train a vanilla FM in a basic FTRL setting but it was shown to be rather slow and less accurate in practice
* This February a formal description of OCCFM which meets the requirements for OCO came out (Lin, 2018)
* This August an approach based on a modified FTRL came out (Luo, 2018), claming to be much faster than OCCFM


+++
title = "Twitter Sentiment Trading"
date = 2021-01-03
[taxonomies]
tags = ["finance","nlp","algo-trading"]
+++

# Twitter Sentiment Trading


The team for this project explored the use of *sentiment analysis* on financial tweets on Twitter. Sentiment Analsyis is a branch of Natural Language Processing that involves determining the *sentiment* of text - in this case whether a tweet is positive or negative (bullish or bearish)  on financial twitter data. In doing so, they explored the use of different classification methods (SVMs, Naive Bayes) and word embedding methods such as *FinBert* and *ULMFiT* (since words are text, and machine learning models require numeric data, text needs to be converted into a suitable numeric representation  - word embeddings). Finally, they backtested a simple trading strategy based on this derived sentiment.


<img src = '/2020/projects/kmeans.png' class='.img-fluid' width=40% height=40%>

<img src = '/2020/projects/trades.png' class='.img-fluid' width=57% height=100%>


A Google Colab notebook is available [here](https://colab.research.google.com/drive/1oh1ZYbRH2nexJcGBBdXvLD5Xg9_Mmkyd)

And the slides to their presentation are available [here](https://docs.google.com/presentation/d/1hnwXuI0S4lTMHgPMH1LqblaLq5dqOP-aNH8PFqpm1lQ/edit?usp=sharing)


[Github Repo](https://github.com/sanj909/DSS_Project_08-2020)


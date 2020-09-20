+++
title = "Kaggle Clone - Data Science Competition Platform"
date = 2020-06-22

[taxonomies]
tags = ["go"]
+++

# Kaggle Clone - Data Science Competition Platform

A rudimentary Kaggle Clone was developed for the purposes of organising Kaggle competitions within the society and as a prototype for a student research paper.

<img src = '/2019/kaggle-clone-main.png' class='.img-fluid' width=40% height=40%>
<img src = '/2019/kaggle-clone-main-2.png' class='.img-fluid' width=40% height=40%>

+ [Website](https://mlatlse-datathon.herokuapp.com/)
+ [Repository](https://github.com/collaborai/gopot-prototype)
+ ["PoET: design and implementation of collaborative machine learning"](https://github.com/collaborai/collabor.ai/blob/master/PoETPaper.pdf)

A group of actors on a trustless network working on an identical machine learning problem could achieve collective performance gains if they could exchange models, and were rewarded according to their contribution (i.e. model performance) to the task. However moral hazard and informational asymmetry prevents this exchange - for example, any actor could misreport the performance of their model. The proposed solution is to use a new blockchain mechanism: predictions are fed into an ensemble model , hence the ensemble validation score against some preagreed valiation set is the ("Proof of Ensemble Training"). The reward mechanism to each actor on the network, would be some preagreed measure of feature importance in the ensemble model (thus the contribution of each actor).

For this prototype, a decentralisated network is not implemented. A Flask frontend is used (which also computes validation scores), which sends the results to a Go backend, which does further validation before updating a centralised Firebase database used as persistence (for the blockchain).



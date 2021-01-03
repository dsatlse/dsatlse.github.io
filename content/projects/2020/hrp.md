+++
title = "Portfolio Optimisation - Hierarchial Risk Parity"
date = 2021-01-03
[taxonomies]
tags = ["finance","machine-learning"]
+++

# Portfolio Optimisation - Hierarchial Risk Parity

The team for this project explored the use of *Hierarchial Risk Parity*. The Mean-Variance based portfolio optimisation (Markowitz Portfolio Theory), studied in a standard finance course such as *FM212* or *FM213* involves the construction of a portfolio based on the covariance matrix. However, the covariance matrix only accounts for the covariance between *pairs of assets*.  Hierarchial Risk Parity uses hierarchial clustering to build clusters of assets - accounting for possible factors, then calculates covariances between clusters from which a portfolio can then be constructed.

<img src = '/2020/projects/DBar-Matrix.gif' class='.img-fluid' width=40% height=40%>

<img src = '/2020/projects/clusters.png' class='.img-fluid' width=40% height=40%>


A Google Colab notebook is available [here](https://colab.research.google.com/drive/1IpYLBmVwAnL1g_99o5BIhcZ9V6_Ij0j7)

And the slides to their presentation are available [here](https://docs.google.com/presentation/d/1BgqQtQWeMMhV2k7NSFyCR3vlgHHoQkqmIqY7i4BorGw/edit?usp=sharing)

### References

+ [https://gmarti.gitlab.io/qfin/2018/10/02/hierarchical-risk-parity-part-1.html](https://gmarti.gitlab.io/qfin/2018/10/02/hierarchical-risk-parity-part-1.html)

+ [https://hudsonthames.org/an-introduction-to-the-hierarchical-risk-parity-algorithm/](https://hudsonthames.org/an-introduction-to-the-hierarchical-risk-parity-algorithm/)

+ [https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2708678](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2708678)

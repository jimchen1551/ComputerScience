---
Created: [[2022-11-26]]
Aliases: 
Types: Card
Tags: 
- 
---
# Naive Bayes model
$$\mathbf{M}(q)=\arg\max_{l\in levels(t)}P(t=l)\times\prod_{i=1}^mP(q[i]|t=l)$$
, where 
1. $t$ is a target feature with a set of levels, $levels(t)$
2. $q$ is a query instance with a set of descriptive features, $q[1], \dots, q[m]$
- returning a **MAP** prediction ([[Maximum a posteriori]])
- computing the **posterior probabilities** for the **levels of the target feature** under the assumption of **conditional independence** b/w descriptive features
- robust to **data fragmentation** and the **curse of dimensionality** (with small data or with sparse data)
- successful in text analytics

---
Created: [[2022-11-25]]
Aliases: 
Types: Card
Tags: 
- 
---
# Bayes' theorem
$$P(A|B)=\frac{P(B|A)P(A)}{P(B)}$$
$$\displaystyle P(A_i|B)=\frac{P(B|A_i)P(A_i)}{\Sigma_{j=1}^nP(B|A_j)P(A_j)}=\eta\cdot P(B|A_i)\cdot P(A_i)$$
$$\eta=\frac{1}{P(B)}=\frac{1}{\Sigma_{j=1}^nP(B|A_j)P(A_j)}$$
, where $\eta$ is normalization constant
- the probability that an event has happened given a set of evidence for it is equal to the probability of the evidence being caused by the event multiplied by the probability of the event itself

## Generalized Bayes' theorem
$$P(t=l|q[1],\dots, q[m])=\frac{P(q[1],\dots, q[m]|t=l)P(t=l)}{P(q[1],\dots, q[m])}$$
, where $t$ for target features and $q$ for a set of descriptive features from a query instance

1. Prior probability: 
   $$P(t=l)$$
2. Joint probability: 
   $$P(q[1],\dots, q[m])=P(q[1])P(q[2]|q[1])\dots P(q[m]|q[m-1]\dots q[1])$$
3. Likelihood: 
   $$P(q[1],\dots, q[m]|t=l)=P(q[1]|t=l)\dots P(q[m]|q[m-1]\dots q[1],t=l)$$
4. Posterior probability (prediction):
   $$P(t=l|q[1],\dots, q[m])$$
## Bayesian vs Frequentist
- Frequentist: 
  1. Only follow the prior theory
  2. Real is rational, and rational is real
  3. Explain data as the frequency (likelihood) of distribution
  - e.g., [[Maximum likelihood|MLE]]

- Bayesian: 
  1. Assume a prior theory as $\theta$ 
  2. Observe the data $D$ 
  3. Adjust the theory with the likelihood $D|\theta$ 
  4. Get the posterior theory as $\theta|D$ 
  - e.g., [[Maximum a posteriori|MAP]]

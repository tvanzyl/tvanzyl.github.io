---
author: Terence L van Zyl
title: Representation Learning
date: 2021-03-08
description: Representation Learning
math: true
---

The recent paper by Variawa and van Zyl *inter al.* (2022) [[ref]](https://ieeexplore.ieee.org/abstract/document/9709840) looks at transfer learning and deep metric learning for galaxy morphology classification. 

<!--more-->

The most exciting result from this paper is that metric learning outperformed traditional classification on the minority classes. Prevalence of minority classes seems to be a characteristic of crowdsourced data, a red flag raised in this study and requiring consideration in similar projects. 

The performance of learning algorithms massively depends on the representations they receive as input. Representation learning tries to train machine learning algorithms to learn useful representations, such as those that are interpretable, capture invariance, incorporate latent features, or can be used for transfer learning. From this perspective, deep neural networks are representation learning models. At a high-level, a typical supervised neural network has two components, (1) an encoder and (2) a linear classifier.

#### Supervised

- Disentangled Representations

##### Metric Learning

Pseudometrics are measures of quantitative assessment commonly used for comparing. A metric or distance function is a function that gives a distance between each pair of point elements of a set. Such that the number is zero if elements are identical, the number is symetric w.r.t the order of the elements, and the triangular inequality holds.

$d(x,x)=0$
$d(x,y)=d(y,x)$
$d(x,y)<=d(x,z)+d(z,y)$

- Similarity Learning
- Learning to Ranking: Information Retrieval

##### Learning to Order

Order theory investigates the intuitive notion of order using binary relations. It provides a formal framework for describing statements such as "this is less than that" or "this precedes that".

$x<=y$ and $y<=z$ then $x<=z$
$x<=y$ and $y<=x$ then $x=y$
$x<y$ then $~y<x$

- DirectRanker
- Ordinal regression

#### Semisupervised

[](https://medium.com/intuitionmachine/navigating-the-unsupervised-learning-landscape-951bd5842df9)

- Co-training
- Generative
- Adversarial

#### Unsupervised

- Cluster Learning

##### Self-Supervised Learning

- Consistency Regularisation
- Contrastive Learning
- Reconstruction: Autoencoder

##### Generative Learning

P(Z) = P(Z,X,Y)/P(X,Y|Z)
P(X,Y) = P(X)P(Y|X)
P(X|Y) = P(Y|X)P(X)/P(Y)

- VAE
- GAN

#### Other

- RNN, GNN, CNN
- Attention
- Catastrophic forgetting
- Bi-Directional
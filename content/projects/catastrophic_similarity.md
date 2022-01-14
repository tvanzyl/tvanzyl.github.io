---
author: Terence L van Zyl
title: Catastrophic Forgetting in Similarity Learning
date: 2021-03-08
description: Catastrophic Forgetting in Similarity Learning
math: true
---

This research project looks at the impact of catastrophic forgetting and incremental learning in similarity learning.
<!--more-->

Incremental learning is when we continuously update a machine learning model with new objectives (classes or tasks).  The adapted model should ideally improve while losing the least amount of previous information possible. Recent research shows that machine learning models are always affected by catastrophic forgetting during incremental learning when constrained to the above requirements. Catastrophic forgetting is a model losing previous information on old objectives while learning for new objectives. This forgetting results in a good performance on the new objectives and severe performance degradation on the old objectives.  It is essential to understand how different classes or tasks' distributions affect the catastrophic forgetting problem during incremental learning. Catastrophic forgetting could also result from the training setup of the machine learning model. It would be interesting to investigate how different optimizers, the rate of learning, various loss functions, regularisation, and the network model's size affect the rate at which the network forgets during incremental learning. This type of investigation has received little attention and would provide an insight into training setup combinations for incremental learning to reduce catastrophic forgetting.

## Collaborators 

* Jiahao Huo, University of the Witwatersrand 

---
author: Terence L van Zyl
title: WTF Learning
date: 2024-05-22
description: WTF Learning
math: true
---

Machine learning has so many words and ideas that it's becoming increasingly difficult to know what is happening. I have tried to capture some coherence here to aid discussions.

<!--more-->

Some background terms

> - Model: A machine learning model
> - Task: the problem or objective a model is required to solve
> - Skill: the ability of a model to perform a specific task
> - Learning: the process by which a model improves its skill after gaining experience
> - Pretext Task: a contrived task that may lead to learning on the actual task
> - Target: the outcome expected for a given task or pretext task
> - Sample/Example: a single unit of data observed in the learning process
> - Dataset: collection of samples used to train or test a model
> - Training: the process of increasing a model's skill during learning
> - Testing: the process of testing a model's skill during learning
> - Domain: specific area or field of knowledge from which the dataset comes
> - Label/Class: a categorical target associated with a sample in a classification task
> - Classes: the set of labels in a classification task
> - Knowledge: factual information, patterns, and relationships a model has learned
> - Embedding Space: 
> - Attributes:

# Data Distribution Constraints

These are constraints placed on the learning due to the available dataset.

- Supervised learning `dataset includes the task's target`
- Semi-supervised learning `only a subset of the dataset includes the task's target.`
- Unsupervised learning `dataset does not include the task's target.`
- Self-supervised learning `target created from a pretext task.`
- Reinforcement learning `dataset only includes task's target in the last sample.`

# Data Sampling Constraints

The constraints arise due to limitations on how we can sample the dataset.

- (?) Zero-shot learning: `uses class attributes rather than label as a target.`
- One-shot learning `where each class has one training sample.`
- Few-Shot learning: `where each class has fewer than six training samples`
- Continual/Lifelong/Incremental learning `learn new tasks without forgetting old tasks`
- Online learning `training and testing simultaneously`
- Batch learning `training followed by testing in separate activities`
- Open Set learning `test samples from classes unseen during training`

# Approaches To Learning

- Meta-learning `learning to learn more effectively`
- Curriculum learning `next training sample selected according to curriculum`
- Active learning `next training sample actively rather than stochastically selected`
- Domain adaptation `makes a model trained on a source domain perform well on a related target domain`
- Transfer learning ` leverage knowledge gained from one task to improve performance on a related task.`
- Knowledge distillation `transfer knowledge from a complex model (teacher) to a more efficient model (student)`
- Adversarial learning `two models are trained in a competitive setting`
- Contrastive learning `learn by contrasting similar and dissimilar samples`
- Data augmentation `applying various transformations to a dataset to increase diversity`
- Data distillation `creates a synthetic dataset that captures the essential knowledge of a larger dataset`

# Learning Problems

- Representation learning `learns a function that maps samples into an embedding space`
- Metric learning `learns a function that maps samples into an embedded space that preserves the samples' dis/similarity
- Learning-To-Rank `learns a function that maps samples into an embedded space that preserves the samples' rankings.`

- Detection `selects true or false as the task's target`
- Classification `selects one of the classes as the task's target`
- Recognition `detects (true or false) if sample matches a query target.`
- Retrieval `returns all samples that match a query target`

- Anomaly detection
- Out-of-distribution detection `detects instances not from distribution of training - data.`
- Open Set recognition `detects test samples from classes unseen during training.`
- Out-of-domain (OOD) generalization `learns from one or multiple training domains, - to extract a domain-agnostic model which can be applied to an unseen domain.`

## Computer Vision Examples

- Object detection 
- Object tracking 
- Object recognition
- Object re-identification
- Instance segmentation
- Semantic segmentation

- Action/Activity Detection
- Action/Activity recognition

- Depth estimation

- Instance Retrieval
- Recommendation Systems

- Generative models
- Density estimation

# Bla

Rule-based learning
Quantum machine learning
Fairness

+++
description = "About TvZ"
date = "2020-11-02"
aliases = ["about-us", "about-tvz", "cv"]
author = "Terence van Zyl"
+++

#### Representation Learning

Machine learning requires strong priors/predicates, and a smaller amount of empirical risk minimization. Understanding the nature of data will lead to a formulation of appropriate priors/predicates for ML and in doing so allow for improved performance with fewer data. Currently, many approaches such as convolutional neural networks are not explicit about the priors/predicates used and as such cannot exploit this framework. The aim is to understand the nature of data and its structure at a fundamental level by ingesting the mathematical theory and translating it into experiments designs to test the theory. 

##### Transfer Learning

One area that relates directly to representation learning is that of transfer learning. Here we see if priors/predicates on one set of data can be transferred to another. The key question, however, is: What exactly is being transferred in transfer learning? Is it Low-level Features, High-level Features, Initialization, Hyper-parameters, Architecture or Sub-Architectures?

##### Similarity Learning

Another type of representation learning is that employed in similarity learning for Information Retrieval. The idea is to learn an embedding and/or metric which minimises the distance between similar data points and maximises the distance between dissimilar ones. The resulting embedding is a representation of the data. If the challenge of similarity learning was one of fitting points into space: Then finding an embedding that projects the points into 1 or 2 dimensions would be enough. We know it is possible to find a projection of the points into such a small space and achieve perfect mean average precision. However, this embedding would not generalise well to unseen classes in the domain. The real challenge then is finding a set of characteristic features of the domain that are discriminative of classes within the domain. For example colour is a characteristic feature of vehicles but if probably not that discriminative. The number of wheels on the other hand is a discriminative characteristic feature. 

##### Manifold Learning and Dimensionality Reduction

Intrinsic dimension for a data set can be thought of as the number of variables needed in a minimal representation of the data. Dimension reduction is the transformation of data from a high-dimensional space into a low-dimensional space so that the low-dimensional representation retains some meaningful properties of the original data, ideally close to its intrinsic dimension. One approach to simplification is to assume that the data of interest lie on an embedded non-linear manifold within the higher-dimensional space. Manifold learning seeks to find this embedding.

##### Sparse Dictionary Learning

Sparse dictionary representation learning aims to find a sparse representation of the input data that is a linear combination of some basic dictionary atoms as well as those atoms themselves.

##### Autoencoders

Autoencoders learn a representation for a set of data by training a learner to reconstruct its input after passing the data through a learned reduced non-linearity or encoding. The autoencoder tries to generate from the reduced encoding a representation as close as possible to its original input. The reduced encoding is considered to be an embedding of the data.

#### Prescriptive Analytics and Data-Driven Heuristic Optimisation

Data-driven process optimisation and control resides at the intersection of complex adaptive systems modelling and simulation, machine learning and heuristic optimisation. The outcome of which is the realisation of prescriptive analytics models that are applicable in diverse applications ranging from financial portfolio optimisation through predictive maintenance and industrial manufacturing process optimisation to epidemiology. Improving prescriptive analytics requires research into optimal control/reinforcement learning, complex adaptive systems simulation, time-series forecasting, learning representations and surrogate assisted evolutionary algorithms. Prescriptive analytics can lead to optimized decision making, ahead of time, for industrial process improvement. If we can predict (forecast/interpolate/extrapolate) an attribute of a process and infer causation then we can prescribe the set of actions going forward to minimise/maximise our future loss/reward. Arriving at this set of actions requires optimisation to take place.

#### Adaptive Non-parametric Techniques in Spatial-Temporal Data Analysis

Having an accurate heuristic method for determining k in the class of k-NN Kernel Density Estimators will allow us to use these techniques more effectively. However, although k-NN is a powerful tool for density estimation, current heuristics methods for determining k are sub-optimal when used on simulated data sets. In response to this problem, we propose to derive, implement and evaluate the accuracy of a new expectation maximisation algorithm for k selection.

#### Learning Complex Adaptive Systems

The only examples we have of "truly" learning adaptive systems are living organism that has been hypothesised to be complex adaptive signal regulatory systems. The aim is to formulate learning in complex adaptive signal regulatory systems to achieve AI. 


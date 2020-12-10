---
author: Terence L van Zyl
title: Surrogate Assisted Data-Driven Evolutionary Computing
date: 2020-12-10
description: Surrogate Assisted Data-Driven Evolutionary Computing
math: true
---

Interesting applications arises at the intersection of evolutionary computing and machine learning when we capitalise on the strengths of both of these paradigms simultaneously.
<!--more-->

Computational Intelligence, specifically evolutionary computing, has shown substantive utility in the optimisation of complex non-linear systems with numerous positive and negative feedback loops. These non-linear systems are often difficult to optimise directly or generically and often entail long-running simulations to evaluate even with known parameters. 

Recent advances in machine learning, especially deep learning, have demonstrated both analytically and empirically that these models are universal approximators capable of modelling even chaotic systems given sufficient data.

An interesting application arises at the intersection of evolutionary computing and machine learning when attempts are made to capitalise on the strengths of both of these paradigms simultaneously. In this new solution space to the above mentioned non-linear complex systems requiring optimisation, machine learning is introduced as a surrogate for the long-running simulations. These surrogates allow for several performance enhancements to the current metaheuristic optimisation frameworks. 

For instance, a surrogate machine learning model might be introduced into a genetic algorithm (GA) and in so doing, allow the GA to make substantially more evaluations of its heuristic function. Further, the surrogate might act as a sort of tabu search within the neighbourhood around already explored portions of the optimisation landscape. 

Both evolutionary computational algorithms and machine learning are active areas of research with substantive advances in recent literature with the introduction of deep learning and algorithms like CMA-ES. Further, these algorithms and the combination of them in the form of surrogate assisted data-driven optimisation has lead to numerous recent advances in a variety of applications ranging from drug discovery to chemical batch plant optimisation.

## Collaborators

* Dr Matthew Woolway, Imperial College London


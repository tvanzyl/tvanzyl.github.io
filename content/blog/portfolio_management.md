---
author: Terence L van Zyl
title: Machine Learning in Finance
date: 2021-03-08
description: Machine Learning in Finance
math: true
---

This research project looks at the intersection of finance and machine learning.
<!--more-->

#### Improving DRICORN-K using Recurrent Neural Networks and Similarity learning 

Online Portfolio Selection is a fundamental problem in Computational Finance. Our recent pattern-Matching method, DRICORN-K: A Dynamic RIsk CORrelation-driven Non-parametric Algorithm for Online Portfolio Selection, has shown itself to be a promising technique. DRICORN-K, the current state of the art, considers systematic risk and leads to better investment returns, especially in volatile markets. However, there is still a gap concerning the estimation of volatility and computational overhead associated with pattern-matching. This research project will investigate machine learning and similarity learning to improve the DRICORN-K algorithm and other pattern-matching algorithm
1. To what extent can we improve return and volatility estimation using deep recurrent neural networks for online portfolio selection.
2. To what extent can similarity learning be employed to improve inter-temporal pattern matching in financial time series over for instance classical methods such as dynamic time warping (DTW).


#### Reinforcement Learning for Inter-temporal Portfolio Choice problems

The mean-variance portfolio optimisation approach, commonly thought of as risk versus return or greed versus fear, is inherently solved as a myopic single-period problem. In reality, we sometimes think of investment problems as involving longer horizons with intermediate portfolio rebalancing with associated transaction costs and potential consumption. The most straightforward way to address these issues is to explicitly formulate the problem in terms of inter-temporal expected utility maximisation [1]. We consider the consumption-investment problem with a constant relative risk aversion preference function, who possesses noisy information about a stock's prospects. It has been shown that information can significantly alter consumption and asset allocation decisions [2]. This problem is well suited to reinforcement learning or stochastic control/dynamic programming.  To this end, we propose the use of reinforcement learning or stochastic control/dynamic programming to allocate between cash and an index to maximise utility for an agent.

#### Outperforming An Index such as the S&P 500 or JSE Top 40

The mean-variance paradigm (MVP) of Markowitz (1952) is the most common formulation of portfolio choice problems. We have a set of N risky assets and a risk-free asset with a known return. The problem is to allocate wealth amongst the assets to minimise the risk for a given expected return. Index tracking funds are passive investment instruments, often traded as an exchange-traded fund (ETF). An ETF has an associated risk derived from the weighting of its constituent assets. An alternate formulation of MVP would be to maximise return for a given expected risk. This research project will formulate an alternate portfolio for index-tracking ETF's assets to capture the same expected risk whilst achieving a maximised reward. We can further extend the project to use various machine learning and statistical models to estimate both returns and risk in arriving at an optimal portfolio. 

## Collaborators

* Andrew Paskaramoorthy, University of the Witwatersrand


---
author: Terence L van Zyl
title: Self-supervised Continual Learning
date: 2024-05-22
description: Self-supervised Continual Learning
math: true
---

Ideally machine learning models should be capable of learning without *"explicit"* supervison and do so continously without forgetting what they have previously learned [\[1\]][1].

<!--more-->

However, neither of these two problems are satisfactorily solved in deep learning. 

Tha main aim then is to uderstand the circumstance under which self-supervised continous learning might be achieved. This leads to several streams of thought:

1. What makes a good representation?
2. What makes a good represenation learner?
3. How do we protect what has been learnt before?
4. How do we know what has been learn before?
5. How do we achieve memorisation along side generalisation [\[2\]][2]?

An entity has several attributes some of which are relationships with other entities. An attribute refers to a property, quality, aspect or characteristic of an entity that can be measured (quantitative) or observed (qualitative). However, we cannot measure the attributes of entities directly instead we use a sensor to make a observation of some phenomenon and then use these as proxies to infer the attribute.

The attributes of entities that coincide with one another lead to natural orderings of entities and an opportunity for compression.

## Good Representations

Why representations matter is a question of importance. Is it mearly a matter of convenience that vectors match type of compuations we can do easily on the von-neuman architecture? Or is there some inherent realtionship between perception and vector represenations in hilbert space?

Representation learning learns a transformation $f:\mathbb{R}^D\rightarrow \mathbb{R}^E$ where $D$ is the dimension of the input and $E$ is the dimension of the embedding.

Assume that $x \in X$ and $x^- \in X$ are observation(s) of two diffent entities e.g. a single image or two images of two diffent people. 

$X$ has symmetries $s(X)$ imposed by its environment. s.t $x^+ = s(x)$ is a seperate observation of the entity $x$. e.g. an image of the person at a different time or from a different angle.

Let $z = f(x)$ and $z^+ = f(x^+)$ be embeddings of $x$ and $x^+$ i.e. two embeddings of the same entity at different symmetries and $z^- = f(x^-)$ be an embedding of a diffent entity.

A classification function $c = c(z)$ results in a type system or assigns a class to $x$ through $z$. Where $c(\cdot)$ might be linear or non-parametric.

$H(\cdot)$ is entropy.

### Neccesary Characteristics

- Representation $z$ should be aligned.
  - $z^+ \approx z \not\approx z^-$
- Efficient/Compact: $H(Z) \ll H(X) \implies E \ll D$
- Representation $z$ should be covariant under symmetry $s(\cdot)$ 
  - There exists a function $g$ such that $g(z, z^+) = s$
- Aligned and Efficient representations implies:
  - Representation $z$ should display subtyping: is-a
  - Representation $z$ should be composable: has-a

and

- irrelevant details are abstracted away???
<!-- - Representation learner $f$ is covariant under symmetry $s(X)$ 
  - if there exists a function $g$ such that $g(f\circ s(X), f(X)) = s$ -->
- Representation learner $f$ is invariant under symmetry $s(\cdot)$ 
  - if $z^+ \approx z \not\approx z^-$. 

#### Representation $z$ should be covariant under symmetry $s(\cdot)$ 

Means that the embedding $z^+ = f\circ s(x)$ contains information that allows us to recover the symetry that was applied when compared to $z$.

#### Representation learner $f$ is invariant under symmetry $s(X)$ 

Means the embedding $z^+ = f\circ s(x)$ is closer to to $z$ than any other $f(x^-)$.

#### Aligned 

Representation $z$ is aligned with $z^+$ and $z^-$ if $z^+ \approx z$ and $z^- \not\approx z$. By $\approx$ and $\not\approx$ we mean that $\mathbb{E}[|z,z^+|_2^2] < \mathbb{E}[|z,z^-|_2^2]$

### Desirable Characteristics

- Uniform
- Facilitating Transfer Learning: Reusability and Domain Adaptation
- Sparse
- Distibuted
- Disentangled

and 

- Representation learner $f$ is equivariant under symmetry $s(X)$ 
  - if $f\circ s(X) = s\circ f(X)$.

```
1. Can we use catastrophic forgetting to regularise energy based non-contrastive learning?
2. Can a neural network be trained to predict how recently it observed specific example? (Recency Encoding)
3. Can we use incremental learning on a single camera at a time to ...?
```

### Learning by reconstruction 

$$\argmin_{\theta_e,\theta_d} \mathbb{E}[|\hat{x},x|_2^2]$$ 
where $\hat{x} = \mathrm{dec}_{\theta_d} ( z=\mathrm{enc}_{\theta_e} (x) )$
produces uninformative embeddings $z$ for perception due to the "details" being learned last [\[3\]][3]. Intersingly it is clear that with sufficent training eventually the learning moves from a lossy towards a lossless regium over time.

Representaions are:
1. Compact 
2. Covariant

Represenation aren't gaurenteed to be:
1. Aligned
2. 

The learner is not gauranteed to be 
1. Invariant




bibliography:
- [1]: <https://www.cell.com/trends/cognitive-sciences/fulltext/S1364-66132030219-9> "Embracing Change: Continual Learning in Deep Neural Networks"
- [2]: <https://proceedings.mlr.press/v70/arpit17a/arpit17a.pdf> "A Closer Look at Memorization in Deep Networks"
- [3]: <https://arxiv.org/pdf/2402.11337#page=2.29> "Learning by Reconstruction Produces Uninformative Features For Perception"
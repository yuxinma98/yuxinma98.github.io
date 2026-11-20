---
title: "Any-dimensional learning and size generalization"
date: 2026-11-20
summary: "We present a theoretical framework for understanding size generalization in neural networks that take inputs of arbitrary size. We then apply this framework to weight-space learning, where it motivates model modifications that achieve strong size generalization in practice."
versions:
  - date: 2026-11-20
    location: "Minisymposium *Modern Data Science Perspectives on Geometric Representations and Manifold Learning*, SIAM Conference on Mathematics of Data Science (MDS26)"
    length: "25 min"
    slidesUrl: "/slides/2026-anydim-learning-25/"
  - date: 2026-11-10
    location: "Graduate Student Seminar, Department of Applied Math and Statistics, Johns Hopkins University"
    length: "45 min"
    slidesUrl: "/slides/2026-anydim-learning/"
papers:
  - publications/2025-transferability
  - publications/2026-transferable-graph-metanetworks
draft: false
---
Many modern architectures — including DeepSets, graph neural networks, and transformers — are designed to process inputs of arbitrary size. These models have a desirable feature: they can be trained on small inputs and deployed on larger ones. Yet the theoretical conditions under which such size generalization succeeds or fails remain poorly understood.

In this talk, we reveal a fundamental mechanism behind size generalization: many of these models encode a hidden inductive bias about relationships between objects of different sizes. Specifically, they parameterize functions that are continuous with respect to a pseudometric on the space of inputs across all sizes. When this pseudometric captures equivalences and proximity between objects of different sizes, performance transfers between objects that differ in size but are close under the pseudometric. This perspective yields an approximation and generalization theory in the any-dimensional setting, and lets us determine precisely for which tasks and data distributions a model trained on small inputs will generalize to large ones. It also inspires new architectures, and modifications of existing ones, that achieve size generalization on tasks where standard models fail.

We will also present an application of this theory to weight-space networks (or meta networks), which take the weights of another neural network as input and predict its properties. We propose principled modifications to existing metanetworks that achieve, to our knowledge, the first robust and provable size generalization in weight-space learning. Beyond demonstrating the practical relevance of our theory, this work opens a new direction for GNN transferability in weight-space learning and reveals an intriguing link to the infinite-width limits of neural network training dynamics.

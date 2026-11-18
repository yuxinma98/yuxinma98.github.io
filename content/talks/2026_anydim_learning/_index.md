---
title: "Any-dimensional learning and size generalization"
date: 2026-11-10
location: "Graduate Student Seminar, Department of Applied Math and Statistics, Johns Hopkins University, Baltimore"
slidesUrl: "/slides/2026-anydim-learning/"
draft: false
---
**Abstract**: Many modern architectures — including DeepSets, graph neural networks, and transformers — are designed to process inputs of arbitrary size. These models have a desirable feature: they can be trained on small inputs and deployed on larger ones. Yet the theoretical conditions under which such size generalization succeeds or fails remain poorly understood.

In this talk, we reveal a fundamental mechanism behind size generalization: many of these models encode a hidden inductive bias about relationships between objects of different sizes. Specifically, they parameterize functions that are continuous with respect to a pseudometric on the space of inputs across all sizes. When this pseudometric captures equivalences and proximity between objects of different sizes, performance transfers between objects that differ in size but are close under the pseudometric. This perspective yields an approximation and generalization theory in the any-dimensional setting, and lets us determine precisely for which tasks and data distributions a model trained on small inputs will generalize to large ones. It also inspires new architectures, and modifications of existing ones, that achieve size generalization on tasks where standard models fail.

We will also present an application of this theory to weight-space networks (or meta networks), which take the weights of another neural network as input and predict its properties. We propose principled modifications to existing metanetworks that achieve, to our knowledge, the first robust and provable size generalization in weight-space learning. Beyond demonstrating the practical relevance of our theory, this work opens a new direction for GNN transferability in weight-space learning and reveals an intriguing link to the infinite-width limits of neural network training dynamics.

[Slides](/slides/2026-anydim-learning/)

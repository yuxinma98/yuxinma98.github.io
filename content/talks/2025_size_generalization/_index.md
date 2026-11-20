---
title: "Some thoughts on size generalization"
date: 2025-08-12
summary: "Models such as DeepSets, GNNs, and transformers accept inputs of any size, but what makes them generalize from small training inputs to larger test inputs? I argue that two ingredients matter: the task must align with the model, and the training and test distributions must be similar as measured by the model's inductive bias."
versions:
  - date: 2025-08-12
    location: "Graph Learning Meets Theoretical Computer Science Workshop, Simons Institute"
    length: "15 min"
    slidesUrl: "/files/2025-08_size-generalization_Simons.pdf"
papers:
  - publications/2025-transferability
draft: false
---
This talk explores the question: For existing models capable of handling inputs of arbitrary sizes (e.g. DeepSet, GNN, transformer), what properties of the data and task enable effective size generalization? My answer involves two key points: (1) task-model alignment; (2) training and test distributions are “similar” relative to the model’s inductive bias.

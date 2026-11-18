---
title: "Research"
aliases: ["/about/"]
---
My current research has been revolving around the following topics:

* **Any-dimensional Learning and Size Generalization**: Architectures like transformers, graph neural networks (GNNs), and DeepSets are designed to handle inputs of varying sizes with fixed-size learnable weights. My research tries to understand their ability to generalize out-of-distribution across sizes: training on small-size inputs and performing well on large-size ones. 
    * We proposed mathematical frameworks to understand the *structure* of the input space of these neural networks, modelling the relationship between objects of different sizes, and to understand the neural network's inductive bias on such structure [[1]](https://arxiv.org/abs/2505.23599) [[2]](https://yuxinma98.github.io/talks/2025_size_generalization/).
    * We apply the theoretical understanding to practice: we design principled modifications on existing neural network architectures, to achieve effective size-generalization with theoretical guarantees. 
    See [[3]](https://arxiv.org/abs/2610.00420) for application to weight-space learning.
* **Scalings and Hyperparameter Transfer**: With different choice of scalings of the hyperparameters with respect to model width/depth (i.e. parameterizations), models of different sizes are related to each other in very different ways. Choice of parameterizations such as $\mu$P and CompleteP were derived so that they have well-behaved infinite-width/depth limit, and so models of different sizes are similarly behaved. This allows hyperparameter transfer (tuning on smaller-size neural networks and directly use on larger ones.) While the existing work focus on understanding the limit behavior in a probabilistic way, we find an interesting connection with the algebraic *structure* of the weight space, modelling the relationship between weights of narrower and wider networks.
    * We leverage the connection to design an algorithm for principled *upscaling* neural networks: using a trained smaller model to initialize the training of a larger one [[4]](https://arxiv.org/abs/2602.10545).
    * We also use the connection to understand the distribution of trained weights, so as to understand size-generalization in weight-space learning [[3]](https://arxiv.org/abs/2610.00420). 
* **Random Matrix Theory and Spectral Algorithms**: Outside neural networks, I'm also interested in spectral algorithms in the low-rank recovery problems in high-dimensional statistics. I'm interested in the symmetry considerations underlying the algorithmic design, and the use of random matrix theory to characterize the performance.
    * In [[5]](https://arxiv.org/abs/2505.12528), we propose a tunable spectral algorithm for Planted Clique problem with a learnable part.


Related to the above, I'm also broadly interested in the following topics:
* Symmetries in neural network architectures and algorithms in low-rank recovery
* Various ways to understand limiting behavior of neural networks and their training dynamics under the randomness of initialization (law-of-large-number of central-limit theorem analysis, statistic physics, random matrix theory)
* Theory of scaling laws
* "Learning an algorithm" that provably outperform existing ones

If you share an interest in any of these, I would be delighted to connect.
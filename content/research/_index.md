---
title: "Research"
aliases: ["/about/"]
---
My current research focuses on the following topics, with links to my related papers and talks:

* **Any-dimensional Learning and Size Generalization**: Architectures such as transformers, graph neural networks (GNNs), and DeepSets process inputs of varying sizes using a fixed set of learnable weights. I study their ability to generalize out of distribution across sizes: training on small inputs and performing well on much larger ones.
    * To understand the mechanism behind size generalization, we propose mathematical frameworks that capture the *structure* of the input spaces of these networks, modeling how objects of different sizes relate to one another, and that characterize the networks' inductive biases with respect to this structure [[1]](https://arxiv.org/abs/2505.23599) [[2]](https://yuxinma98.github.io/talks/2025_size_generalization/).
    * We put this theory into practice by designing principled modifications to existing architectures that achieve effective size generalization with theoretical guarantees.
    See [[3]](https://arxiv.org/abs/2610.00420) for an application to weight-space learning.
* **Scaling and Hyperparameter Transfer**: How hyperparameters are scaled with model width and depth (i.e., the parameterization) determines how models of different sizes relate to one another. Parameterizations such as $\mu$P and CompleteP are derived to have well-behaved infinite-width and infinite-depth limits, so that models of different sizes behave similarly. This enables hyperparameter transfer: tuning hyperparameters on small networks and reusing them directly on larger ones. 
    * While existing work studies these limits probabilistically, we find an interesting connection to the algebraic *structure* of the weight space, which models the relationship between the weights of narrower and wider networks. We leverage this connection to design a principled algorithm for *upscaling* neural networks, i.e., using a trained smaller model to initialize the training of a larger one [[4]](https://arxiv.org/abs/2602.10545). We also use it to understand the distribution of trained weights, which in turn sheds light on size generalization in weight-space learning [[3]](https://arxiv.org/abs/2610.00420).
* **Random Matrix Theory and Spectral Algorithms**: Beyond neural networks, I am interested in spectral algorithms for low-rank recovery problems in high-dimensional statistics, particularly the symmetry considerations underlying their design and the use of random matrix theory to characterize their performance.
    * In [[5]](https://arxiv.org/abs/2505.12528), we propose a tunable spectral algorithm with a learnable component for the planted clique problem.


More broadly, I am also interested in:
* Symmetries in neural network architectures and other algorithmic design
* Different approaches to understanding the limiting behavior of neural networks and their training dynamics under random initialization (law of large numbers and central limit theorem analyses, statistical physics, random matrix theory)
* Theory of scaling laws
* "Learning algorithms" that provably outperform existing traditional algorithms

If you share any of these interests, I would be delighted to connect.

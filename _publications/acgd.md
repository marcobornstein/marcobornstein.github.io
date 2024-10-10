---
title: "Escaping From Saddle Points Using Asynchronous Coordinate Gradient Descent"
collection: publications
category: manuscripts
permalink: /publication/acgd
excerpt: null # 'This paper is about the number 1. The number 2 is left for future work.'
date: 2022-11-08
venue: 'arXiv'
slidesurl: null # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2211.09908'
citation: null # 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Large-scale non-convex optimization problems are expensive to solve due to computational and memory costs. To reduce the costs, first-order (computationally efficient) and asynchronous-parallel (memory efficient) algorithms are necessary to minimize non-convex functions in machine learning. However, asynchronous-first-order methods applied within non-convex settings run into two difficulties: (i) parallelization delays, which affect convergence by disrupting the monotonicity of first-order methods, and (ii) sub-optimal saddle points where the gradient is zero. To solve these two difficulties, we propose an asynchronous-coordinate-gradient-descent algorithm shown to converge to local minima with a bounded delay. Our algorithm overcomes parallelization-delay issues by using a carefully constructed Hamiltonian function. We prove that our designed kinetic-energy term, incorporated within the Hamiltonian, allows our algorithm to decrease monotonically per iteration. Next, our algorithm steers iterates clear of saddle points by utilizing a perturbation sub-routine. Similar to other state-of-the-art (SOTA) algorithms, we achieve a poly-logarithmic convergence rate with respect to dimension. Unlike other SOTA algorithms, which are synchronous, our work is the first to study how parallelization delays affect the convergence rate of asynchronous first-order algorithms. We prove that our algorithm outperforms synchronous counterparts under large parallelization delays, with convergence depending sublinearly with respect to delays. To our knowledge, this is the first local optima convergence result of a first-order asynchronous algorithm for non-convex settings.
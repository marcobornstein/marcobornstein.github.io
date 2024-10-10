---
title: "Comfetch: Federated Learning of Large Networks on Constrained Clients via Sketching"
collection: publications
category: manuscripts
permalink: /publication/commfetch
excerpt: null # 'This paper is about the number 1. The number 2 is left for future work.'
date: 2023-09-30
venue: 'arXiv'
slidesurl: null # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2109.08346'
citation: null # 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Federated learning (FL) is a popular paradigm for private and collaborative model training on the edge. In centralized FL, the parameters of a global architecture (such as a deep neural network) are maintained and distributed by a central server/controller to clients who transmit model updates (gradients) back to the server based on local optimization. While many efforts have focused on reducing the communication complexity of gradient transmission, the vast majority of compression-based algorithms assume that each participating client is able to download and train the current and full set of parameters, which may not be a practical assumption depending on the resource constraints of smaller clients such as mobile devices. In this work, we propose a simple yet effective novel algorithm, Comfetch, which allows clients to train large networks using reduced representations of the global architecture via the count sketch, which reduces local computational and memory costs along with bi-directional communication complexity. We provide a nonconvex convergence guarantee and experimentally demonstrate that it is possible to learn large models, such as a deep convolutional network, through federated training on their sketched counterparts. The resulting global models exhibit competitive test accuracy over CIFAR10/100 classification when compared against un-compressed model training.

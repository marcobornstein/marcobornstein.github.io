---
title: "Large-Scale Distributed Learning via Private On-Device LSH"
collection: publications
category: conferences
permalink: /publication/pghash
excerpt: null # 'This paper is about the number 3. The number 4 is left for future work.'
date: 2023-12-07
venue: 'Thirty-Seventh Annual Conference on Neural Information Processing Systems (NeurIPS)'
slidesurl: null # 'http://academicpages.github.io/files/slides3.pdf'
paperurl: 'https://proceedings.neurips.cc/paper_files/paper/2023/file/34345e243156da67605d4b63d71c8d98-Paper-Conference.pdf'
citation: null #'Your Name, You. (2015). &quot;Paper Title Number 3.&quot; <i>Journal 1</i>. 1(3).'
---

Locality-sensitive hashing (LSH) based frameworks have been used efficiently to select weight vectors in a dense hidden layer with high cosine similarity to an input, enabling dynamic pruning. While this type of scheme has been shown to improve computational training efficiency, existing algorithms require repeated randomized projection of the full layer weight, which is impractical for computational- and memory-constrained devices. In a distributed setting, deferring LSH analysis to a centralized host is (i) slow if the device cluster is large and (ii) requires access to input data which is forbidden in a federated context. Using a new family of hash functions, we develop one of the first private, personalized, and memory-efficient on-device LSH frameworks. Our framework enables privacy and personalization by allowing each device to generate hash tables, without the help of a central host, using device-specific hashing hyper-parameters (e.g. number of hash tables or hash length). Hash tables are generated with a compressed set of the full weights, and can be serially generated and discarded if the process is memory-intensive. This allows devices to avoid maintaining (i) the fully-sized model and (ii) large amounts of hash tables in local memory for LSH analysis. We prove several statistical and sensitivity properties of our hash functions and experimentally demonstrate that our framework is competitive in training large-scale recommender networks compared to other LSH frameworks which assume unrestricted on-device capacity.
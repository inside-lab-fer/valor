---
title: "Fast simulations on domains of changing shape"
ref: vlah-camwa
summary: "A paper in Computers & Mathematics with Applications presents reduced order models that use deep neural networks to learn the domain description on their own."
image: /assets/img/vijesti/vlah-camwa.png
image_alt: "Velocity field of flow in a channel with a widening and an elliptic obstacle"
image_caption: "Solution of channel flow past an obstacle on a domain of varying shape."
---
The paper **Reduced order modeling of partial differential equations on parameter-dependent domains using deep neural networks** (M. Bukač, I. Mikuš, B. Muha, D. Vlah) has been published in **Computers & Mathematics with Applications** (vol. 216, 2026, pp. 282–300). It is available at [doi.org/10.1016/j.camwa.2026.05.008](https://doi.org/10.1016/j.camwa.2026.05.008), with a preprint at [arXiv:2407.17171](https://arxiv.org/abs/2407.17171).

Partial differential equations often depend on parameters and must be solved many times. Reduced order models learn from precomputed solutions and then quickly approximate the solution for new parameters. When the domain itself changes, for example the shape of a blood vessel or the position of an obstacle in a channel, a good description of the domain is needed, which is hard when the shape is complex or changes topology.

The authors propose a framework in which deep neural networks extract the domain description from data, without user-defined control points and without a finite-element mesh, a common situation in biomedical applications. Both the solution and the domain are thus compressed into a low-dimensional latent representation.

The research was partly funded by the VALOR project.

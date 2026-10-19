---
title: "Stable long-horizon prediction of partial differential equation solutions"
ref: equadiff-2026
summary: "At Equadiff 2026 in Prague, Domagoj Vlah presented latent-tensor vision transformers for fast and stable prediction of parametric PDE solutions."
image: /assets/img/vijesti/equadiff-2026.png
image_alt: "Reference solution, AE-ViT prediction and error for velocity and pressure fields behind an obstacle"
image_caption: "Reference, model prediction and error at the end of the rollout: the vortex wake is retained."
---
On 30 June 2026 Domagoj Vlah gave the talk **Stable Long-Horizon Prediction of Parametric PDE Solution with Latent-Tensor Vision Transformers** (D. Vlah, I. Mikuš, B. Muha) at **Equadiff 2026** in Prague.

Simulations described by parametric partial differential equations, such as fluid flow around an obstacle, are computationally expensive. Fast surrogate models that predict the solution step by step usually do well over one step, but errors accumulate over long rollouts. The talk presented a model that compresses the solution into a spatial latent tensor, applies a parameter-aware vision transformer to it, and then reconstructs the full field.

On an advection–diffusion–reaction problem the model gives lower error than comparable approaches, and on Navier–Stokes flow past a cylinder a competitive error, while retaining the vortex-wake structure even at the end of a long rollout. Models of this kind are part of the mathematical groundwork of VALOR.

The research was partly funded by the VALOR project.

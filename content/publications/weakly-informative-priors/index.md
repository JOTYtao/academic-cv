---
title: "Weakly Informative Priors Flow Matching for Probabilistic Regional Solar Irradiance Forecasting"
date: "2026-01-01"
authors: ["me", "S. Chen", "J. Fang", "F. Porté-Agel", "M. C. Lam", "M. Li"]
publication_types: ["article-journal"]
publication:
  name: "IEEE Transactions on Sustainable Energy"
  pages: "1–14"
featured: true
selected_work_order: 1
summary: "Physically guided flow matching generates coherent regional solar irradiance ensembles from recent satellite-observed cloud motion."
image:
  preview_only: true
selected_work:
  name: "WIP-Flow"
  paper: "https://doi.org/10.1109/TSTE.2026.3714841"
  paper_label: "Paper"
  github: "https://github.com/JOTYtao/WIP-Flow"
  image_alt: "WIP-Flow architecture for regional ensemble forecasting"
---

[Paper](https://doi.org/10.1109/TSTE.2026.3714841) · [GitHub repository](https://github.com/JOTYtao/WIP-Flow)

## Research question

Cloud advection explains part of a future irradiance field, but clouds also form, change shape, and dissipate. WIP-Flow forecasts the evolving distribution of regional surface solar irradiance from 30 minutes to four hours ahead.

## Approach

An optical-flow advection module with autoregressive correction constructs a weakly informative prior from recent cloud motion. A conditional latent flow-matching model uses satellite-derived clear-sky index and cloud optical thickness to generate ensemble members along a stochastic probability path.

![WIP-Flow architecture for regional ensemble forecasting](featured.png)

*Figure from the WIP-Flow paper.*

[Original figure (PDF)](framework.pdf)

## Results

The paper reports a four-hour CRPS of **47.81 W/m²**. A 20-member regional ensemble took **26 seconds** on one NVIDIA A6000, a **4.96×** speedup over DiffSolar in the reported benchmark. Evaluation also included four independent ground stations and a downstream PV power forecasting task.

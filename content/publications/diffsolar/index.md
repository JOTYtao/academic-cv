---
title: "Prior Knowledge-Guided Residual Diffusion Model for Enhanced Regional-Scale Probabilistic Solar Irradiance Forecasting"
date: "2026-01-22"
authors: ["me", "S. Chen", "T. Du", "M. Li"]
publication_types: ["manuscript"]
publication:
  name: "SSRN preprint"
featured: true
selected_work_order: 5
summary: "Prior-guided residual diffusion models uncertain regional cloud evolution around a smart-persistence forecast."
image:
  preview_only: true
selected_work:
  name: "DiffSolar"
  paper: "https://doi.org/10.2139/ssrn.6113906"
  paper_label: "Preprint"
  github: "https://github.com/JOTYtao/DiffSolar"
  image_alt: "DiffSolar paper figure showing regional residual diffusion forecasting"
---

[Preprint](https://doi.org/10.2139/ssrn.6113906) · [GitHub repository](https://github.com/JOTYtao/DiffSolar)

## Research question

As forecast lead time increases, cloud evolution makes regional solar irradiance difficult to predict with a single deterministic trajectory.

## Approach

DiffSolar combines a smart-persistence baseline with a diffusion model that samples the stochastic residual fields. The denoiser conditions on multiscale spatiotemporal features, and the sampler uses statistics of regional residuals to guide generation.

![DiffSolar paper figure showing regional residual diffusion forecasting](featured.png)

*Figure from the DiffSolar preprint.*

[Original figure (PDF)](framework.pdf)

## Results

For four-hour-ahead forecasts on the satellite-derived benchmark, the public manuscript reports **105.9 W/m² RMSE** and a **continuous ranked probability skill score (CRPSS) of 0.367**.

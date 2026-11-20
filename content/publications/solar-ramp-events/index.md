---
title: "Relaxed Shape Alignment and Temporal Distortion Loss for Improving Solar Ramp Events Prediction"
date: "2026-01-01"
authors: ["me", "S. Chen", "Y. Chu", "M. Li"]
publication_types: ["article-journal"]
publication:
  name: "Energy and AI"
  volume: "26"
  pages: "100881"
featured: true
selected_work_order: 3
summary: "A differentiable training loss targets the shape, timing, and magnitude of abrupt solar irradiance ramps."
image:
  preview_only: true
selected_work:
  name: "RSTLoss"
  paper: "https://doi.org/10.1016/j.egyai.2026.100881"
  paper_label: "Paper"
  github: "https://github.com/JOTYtao/RSTLoss"
  image_alt: "RSTLoss diagram showing shape alignment and temporal distortion"
---

[Paper](https://doi.org/10.1016/j.egyai.2026.100881) · [GitHub repository](https://github.com/JOTYtao/RSTLoss)

## Research question

Rapid changes in solar irradiance can be mistimed or smoothed out when a forecasting model is trained mainly to minimize pointwise error.

## Approach

RSTLoss uses a differentiable, derivative-based alignment term to capture ramp shape and timing. A kernel based on extreme-value behavior increases sensitivity to the magnitude near ramp boundaries. The loss can be used with different forecasting architectures.

![RSTLoss diagram showing shape alignment and temporal distortion](featured.png)

*Figure from the RSTLoss paper.*

[Original figure (PDF)](framework.pdf)

## Results

Across four BSRN datasets and five deep-learning models, the study reports improvements of up to **7.48% in Ramp Score** and **13.17% in Temporal Distortion Index** relative to the compared loss functions.

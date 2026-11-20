---
title: "SolarFusionNet: Enhanced Solar Irradiance Forecasting via Automated Multi-Modal Feature Selection and Cross-Modal Fusion"
date: "2025-01-01"
authors: ["me", "S. Chen", "D. Navarro-Alarcon", "Y. Chu", "M. Li"]
publication_types: ["article-journal"]
publication:
  name: "IEEE Transactions on Sustainable Energy"
  volume: "16"
  issue: "2"
  pages: "761–773"
featured: true
selected_work_order: 2
summary: "Automated feature selection and cross-modal attention integrate satellite imagery, weather observations, and cloud motion."
image:
  preview_only: true
selected_work:
  name: "SolarFusionNet"
  paper: "https://doi.org/10.1109/TSTE.2024.3482360"
  paper_label: "Paper"
  github: "https://github.com/JOTYtao/SolarFusionNet"
  image_alt: "SolarFusionNet architecture with three input modalities"
---

[Paper](https://doi.org/10.1109/TSTE.2024.3482360) · [GitHub repository](https://github.com/JOTYtao/SolarFusionNet)

## Research question

Intraday irradiance forecasts can draw on satellite observations and local meteorology, but useful features and their relationships change with weather conditions.

## Approach

Modality-specific selection units extract informative channels and variables. Recurrent encoders capture temporal structure, and a Gaussian-kernel ConvLSTM models sparse optical-flow cloud motion. Hierarchical cross-modal attention then combines the three streams.

![SolarFusionNet architecture with three input modalities](featured.png)

*Figure from the SolarFusionNet paper.*

[Original figure (PDF)](framework.pdf)

## Results

For four-hour-ahead forecasts, the study reports **37.4–47.6% forecast skill** relative to smart persistence across the evaluated cases.

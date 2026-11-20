---
title: "Improving day-ahead probabilistic solar irradiance forecasting via shape-prior flow matching for numerical weather prediction downscaling"
date: "2026-01-01"
authors: ["me", "S. Chen", "M. Li"]
publication_types: ["article-journal"]
publication:
  name: "Energy and AI"
  volume: "26"
  pages: "100887"
featured: true
summary: "Shape-prior flow matching converts hourly weather-model forecasts into probabilistic 15-minute irradiance trajectories."
image:
  preview_only: true
selected_work:
  name: "SPFlow"
  paper: "https://doi.org/10.1016/j.egyai.2026.100887"
  paper_label: "Paper"
  github: "https://github.com/JOTYtao/SPFlow"
  image_alt: "SPFlow paper figure illustrating probabilistic solar irradiance downscaling"
---

[Paper](https://doi.org/10.1016/j.egyai.2026.100887) · [GitHub repository](https://github.com/JOTYtao/SPFlow)

## Research question

Hourly numerical weather forecasts can miss short-lived irradiance changes that matter for reserves, storage scheduling, and PV integration.

## Approach

SPTransformer estimates a deterministic 15-minute shape prior from coarse weather predictions, satellite-derived meteorology, clear-sky irradiance, and site information. Conditional flow matching samples high-resolution trajectories around this prior to represent unresolved variability.

![SPFlow paper figure illustrating probabilistic solar irradiance downscaling](featured.png)

*Figure from the SPFlow paper.*

## Results

On SURFRAD, SPFlow improved **CRPS by up to 10.9%** relative to the strongest probabilistic baseline. The study also reports better ramp representation and near-nominal empirical interval coverage.

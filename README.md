# Robust Representation Learning under Noise and Distribution Shift

This repository contains a research project studying the robustness of learned representations under structured noise and distribution shift.

## Motivation

In real-world systems (finance, medical imaging, sensor data), signals are noisy, unstable and often non-stationary.

Understanding how learned representations behave under perturbations is critical for building robust predictive models.

## Approach

We adapt an augmentation-noise alignment framework to medical imaging in order to analyze representation stability under controlled corruptions.

We benchmark multiple representation learning methods:

- SimCLR
- MAE
- VICReg
- LeJEPA

## Experimental Design

- Dataset: OrganAMNIST / MedMNIST-C
- Corruptions:
  - Gaussian noise
  - Gaussian blur
- Multiple severity levels

We introduce a residual corruption pipeline parameterized by an alignment strength `α` to stress-test representation robustness.

## Key Findings

- SimCLR remains significantly more stable under high noise
- Reconstruction-based MAE degrades faster under perturbations
- Objective design directly impacts robustness and signal stability

## Quant Perspective

This work can be interpreted as studying **signal robustness under noise**, which is directly relevant to:

- feature stability in financial time series
- robustness of predictive signals
- modeling under distribution shift

## Report

Full report available here:

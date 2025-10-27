# HISTO-UNet: Topology-Aware Medical Image Segmentation with Dual Uncertainty Quantification

This repository contains the implementation for the paper "HISTO-UNet: Topology-Aware Medical Image Segmentation with Dual Uncertainty Quantification".



HISTO-UNet is a novel framework that addresses critical challenges in clinical image segmentation by integrating topology-preserving constraints with a dual uncertainty quantification system. Our approach employs a multi-task objective, combining medial axis (MA) and marker-controlled (MC) topology losses with a Bayesian deep learning methodology to simultaneously capture both data-inherent (aleatoric) and model-specific (epistemic) uncertainty. Through extensive evaluation on three benchmark histopathology datasets, we demonstrate that HISTO-UNet achieves superior segmentation accuracy and produces well-calibrated uncertainty estimates, making it a more reliable tool for clinical applications.

## Key Contributions

-   **Topology Preservation:** Integrates a dual-component loss (MA + MC) to ensure segmentations are structurally and morphologically correct.
-   **Dual Uncertainty Quantification:** Simultaneously estimates both aleatoric (data) and epistemic (model) uncertainty to provide a comprehensive and interpretable measure of prediction confidence.
-   **Novel Multi-Task Objective:** Unifies segmentation, topology, and uncertainty into a single end-to-end training process.

## Framework Overview

The HISTO-UNet workflow processes an input image through a U-Net backbone to produce logits, which are then used to compute three distinct loss components during training. At inference, the model generates both a final segmentation and a corresponding uncertainty heat map.

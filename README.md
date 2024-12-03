# Meningioma Segmentation Using SAM2

This repository contains the code and resources used in the study **"Zero-Shot" General Purpose Segmentation Models Have Comparable Efficacy to Trained Models: An Analysis of the Meta "Segment Anything Model" on Meningioma MRI**. The study evaluates the performance of Meta's Segment Anything Model 2 (SAM2) on meningioma MRI segmentation tasks and proposes strategies for enhancing segmentation accuracy.

## Overview

SAM2 is a zero-shot segmentation model with the potential to automate MRI segmentation. Our study assesses its baseline performance on the 2023 BrATs Preoperative Meningioma Dataset and introduces augmentation methods to improve segmentation results:
- **Interactive Click-Based Augmentation**: Mimics user input with point clicks.
- **Contour-Based Augmentation**: Incorporates tumor boundary information.
- **Directional Consensus Ensembling**: Combines segmentations to boost accuracy.

## Results

- **Baseline Performance**: SAM2 achieved a Dice score of 0.785 in zero-shot mode.
- **Augmentation Strategies**: 
  - Click-Based: Dice score of 0.876
  - Contour-Based: Dice score of 0.872
- **Ensembling**: Directional consensus raised performance to 0.921

Smaller tumors and those without peritumoral edema were challenging for SAM2, requiring further optimization.

## Citation

If you use this code, please cite our paper. 
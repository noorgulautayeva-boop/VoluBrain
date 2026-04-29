# VoluBrain

## Overview
VoluBrain is a deep learning project focused on the segmentation of hippocampal 
structures from 3D MRI images and unsupervised clustering of hippocampus volume 
values to identify potential risk groups for neurodegenerative diseases such as 
Alzheimer's disease (AD).

This project is part of Challenge #3 from the Biomedical Image Analysis course, 
aiming to develop an AI architecture capable of generalizing across multiple 
medical image segmentation tasks.

## Dataset
**Task04_Hippocampus** from the Medical Segmentation Decathlon (MSD):
- 394 3D MRI volumes (263 training / 131 test)
- Modality: T1-weighted MRI
- Target regions: anterior and posterior hippocampus
- Source: Vanderbilt University Medical Center, Nashville, US
- License: CC-BY-SA 4.0 (open access)

## Project Goals
### 1. Segmentation
- Research and implement deep learning architectures (U-Net / nnU-Net) 
  for 3D hippocampus segmentation
- Segment anterior and posterior hippocampus separately
- Evaluate performance using Dice Similarity Coefficient (DSC)

### 2. Volume Extraction
- Extract hippocampus volume values from segmentation output
- Prepare volume data for unsupervised analysis

### 3. Unsupervised Clustering
- Apply k-means clustering on hippocampus volume values
- Determine optimal number of clusters
- Compare clusters to AD/MCI/control thresholds from literature
- Identify patients potentially closer to a risk group

## Repository Structure

| Folder | Description |
|--------|-------------|
| `data/` | Dataset files |
| `notebooks/` | Jupyter notebooks for exploration and analysis |
| `src/` | Source code for segmentation and clustering |
| `results/` | Output results, metrics and visualizations |


## Methods
## References

## Team
- María Martínez Matamoros
- Nurgul Autayeva

- ## Course
Biomedical Image Analysis — 2025/2026

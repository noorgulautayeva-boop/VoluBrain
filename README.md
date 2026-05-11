# VoluBrain

## Overview
VoluBrain is a deep learning project focused on the segmentation of hippocampal 
structures from 3D MRI images and unsupervised clustering of hippocampus volume 
values to identify potential risk groups for neurodegenerative diseases such as 
Alzheimer's disease (AD).

This project is part of Challenge #3 from the Biomedical Image Analysis course, 
aiming to develop an AI architecture capable of generalizing across multiple 
medical image segmentation tasks and enabling accurate hippocampal volume 
extraction for further clinical analysis.

## Dataset
**Task04_Hippocampus** from the Medical Segmentation Decathlon (MSD):
- 390 total MRI volumes  
  - 260 training volumes  
  - 130 test volumes *(not used, as ground truth labels are not available)*
- Modality: T1-weighted MRI
- Image format: NIfTI (`.nii.gz`)  
- Tensor dimension: 3D volumetric images
- Target regions  
  - 0 → Background  
  - 1 → Anterior hippocampus  
  - 2 → Posterior hippocampus
- Source: Vanderbilt University Medical Center, Nashville, US
- License: CC-BY-SA 4.0 (open access)

## Project Goals (review)
### 1. Segmentation
- Research and implement deep learning architectures (U-Net / U-Net++) 
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

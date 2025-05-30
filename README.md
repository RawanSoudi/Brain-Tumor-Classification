# Brain Tumor Classification from MRI Scans
## Overview

This project implements a multi-class classification system for detecting brain tumors in MRI images using this dataset: https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset. The system classifies scans into four categories: glioma, meningioma, pituitary tumor, and no tumor. The implementation includes both custom CNN architectures and transfer learning approaches using VGG16 and ResNet50.

## Dataset

Total Images: 7,023 MRI scans

Classes:

Glioma

Meningioma

Pituitary tumor

No tumor

## Technical Implementation

### Data Preprocessing

Image extensions supported: .jpg, .jpeg, .png

Transformations applied:

Resize images to 224 x 224

Transform images to Tensor

Normalize images using MEAN = [0.485, 0.456, 0.406] , STD = [0.229, 0.224, 0.225] --> standard of ImageNet


### Data Loading

Custom datasets created using ImageFolder

DataLoaders configured with:

  Batch size: 16
  
  Training data shuffled


### Model Architectures

#### Custom CNN:

  Designed from scratch with optimized layers for feature extraction

#### Transfer Learning:

  Fine-tuned VGG16 with pre-trained weights
  
  Fine-tuned ResNet50 with pre-trained weights

### Results

The implemented models achieve classification of brain tumors with the following performance:

Accuarcy Metrics

Comparison between custom CNN and Transfer Learning




# Melanoma Detection Project

This project aims to create a convolutional neural network (CNN) to accurately detect melanoma, a type of skin cancer that is responsible for the majority of skin cancer-related deaths. Early detection is critical, as it significantly increases the chances of survival. By developing a solution that can analyze skin images and assist dermatologists in identifying melanoma, the manual workload involved in diagnosis could be greatly reduced.

## Table of Contents
- Overview
- Tools & Technologies
- Key Insights
- Acknowledgements

## Overview
This dataset consists of 2,357 images representing both malignant and benign skin conditions, sourced from the International Skin Imaging Collaboration (ISIC). The images are categorized based on ISIC classifications, with a balanced representation of the various classes. However, images depicting melanoma and moles are somewhat more prevalent in the dataset.

The dataset used contains images of the following conditions:
- Actinic Keratosis
- Basal Cell Carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented Benign Keratosis
- Seborrheic Keratosis
- Squamous Cell Carcinoma
- Vascular Lesion

To download the dataset, click [here](https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view).

## Tools & Technologies
- Python libraries for data visualization, model training, and testing such as: NumPy, Pandas, Scikit-learn, StatsModels, Seaborn, and Matplotlib
- Jupyter Notebook for development
- TensorFlow for building the CNN
- Version control through GitHub

## Key Insights

### 1. First Model:
In this initial model, we observed significant discrepancies between the training and validation loss around the 19th and 20th epochs, indicating overfitting. The model performed well on the training data but struggled to generalize to the validation set.
   - **Training Accuracy:** 89.29%
   - **Validation Accuracy:** 51.68%

### 2. Second Model with Augmented Data:
By introducing data augmentation, we managed to reduce overfitting. Although the training accuracy remained largely unchanged, the gap between training and validation accuracy decreased, leading to better generalization.
   - **Training Accuracy:** 60.49%
   - **Validation Accuracy:** 54.14%

### 3. Final Model with Class Imbalance Correction:
After addressing class imbalance and continuing to use data augmentation, both training and validation accuracy improved significantly. The model generalized much better, and overfitting was reduced.
   - **Training Accuracy:** 95.44%
   - **Validation Accuracy:** 79.96%



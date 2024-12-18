# Melanoma Detection Assignment
> This assignment is to build a CNN based model which can accurately detect melanoma. This involves training the pre categorized images of different types of skin cancer types and prepare a model to accuratly detect melanoma skin cancer.


## Table of Contents
* [General Info](#general-information)
* [Importing all the important libraries](#importing-libraries)
* [Data Preparation and Initial Assessment](#data-preparation-and-initial-asssessment)
* [Visualize Data](#visualize-data)
* [Model#1 - With Normalization](#model#1)
* [Model#2 - With Data Augmentation, Normalization & Dropout](#model#2)
* [Handle Class Imbalance](#handle-class-imbalance)
* [Model#3 - With Augmented(Class Balanced) Data](#model#3)
* [Model#4 - With Normalization, Dropouts, Regularization & Class balanced data](#model#4)
* [Summary](#summary)* [Summary](#summary)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

**Background**

  This project is part of the PG Program in AI & ML program, specifically within a Deep Learning course.

**Goal**

  To build a CNN based model which can accurately detect melanoma.

**Business Problem**

  Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

**Dataset**

  The dataset consists of 2357 images which were formed from the International Skin Imaging Collaboration (ISIC).

  The data set contains the following skin diseases:

*   Actinic keratosis
*   Basal cell carcinoma
*   Dermatofibroma
*   Melanoma
*   Nevus
*   Pigmented benign keratosis
*   Seborrheic keratosis
*   Squamous cell carcinoma
*   Vascular lesion

## Data preparation and initial assessment
Define default parameters and load dataset

## Visualize the data
Plot images to visualize each class/category

## Define Reusable Functions
Defining functions for all steps in model building, evaluation

## Model#1 - With Normalization

*   CNN model with normalization and three convolution layers
*   No dropout or regularization used in this initial model.

## Model#2 - With Data Augmentation, Normalization & Dropout

*   To mitigate overfitting from previous model, introducing data augmentation and dropouts.
*   CNN model with data augmentation (flip, rotation, Zoom, Brightness & contrast), normalization and three convolution layers with dropouts

## Handle Class Imbalance

*   Identify class imbalance and handle using augmentor

## Model#3 - With Augmented(Class Balanced) Data

*   Model with normalization, three convolutional layers with dropouts.
*   Trained on Augmented/Class Balanced data

## Summary
**Technical Conclusion:**

* Three CNN models were developed and evaluated for skin cancer classification.
* Model 1, without data augmentation or dropout, suffered from overfitting.
* Model 2 incorporated data augmentation and dropout to address overfitting, but resulted in underfitting.
* Model 3 addressed class imbalance using data augmentation via Augmentor, achieving improved training and validation accuracy (93%).
* Despite improvements, the test accuracy remained relatively low (~37%).  Further model complexity or transfer learning is recommended for improved performance.
* The data augmentation strategy using Augmentor effectively balanced the class distribution in the training dataset, which was a key factor in improving model performance.

**Business Conclusion:**

* The developed model demonstrates the potential for automated skin cancer classification.  While the current accuracy (~37% on test data) is not yet suitable for direct clinical use, it represents a foundational step.
* Future improvements focusing on model architecture and larger, more diverse datasets could significantly enhance diagnostic accuracy.
* This technology holds promise for assisting dermatologists in preliminary screenings, potentially leading to earlier detection and improved patient outcomes.
* Further research and development are needed before deployment in a clinical setting.  A more robust model with higher accuracy and validated performance is required.
## Acknowledgements
* Thanks to the instructors from UpGrad and IIITB for guidance and feedback.

## Contact
Created by [@SomasekharGangarapu] - feel free to contact us!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
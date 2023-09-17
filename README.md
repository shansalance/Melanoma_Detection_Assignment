# Melanoma Detection Project

> The objective of this project is to develop a CNN-based model capable of accurately identifying melanoma, a potentially fatal type of skin cancer. Early detection is crucial, as melanoma accounts for 75% of skin cancer-related deaths. Creating a solution that can evaluate images and alert dermatologists to melanoma presence has the potential to significantly reduce manual diagnostic efforts.

## Table of Contents
* [Problem Statement](#problem-statement)
* [Project Pipeline](#project-pipeline)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

## Problem Statement

### Business Context

The dataset consists of 2,357 images depicting both malignant and benign oncological diseases. These images originate from the International Skin Imaging Collaboration (ISIC). They have been categorized based on ISIC classifications, with melanomas and moles having a slight dominance.

The dataset includes the following diseases:

* Actinic keratosis
* Basal cell carcinoma
* Dermatofibroma
* Melanoma
* Nevus
* Pigmented benign keratosis
* Seborrheic keratosis
* Squamous cell carcinoma
* Vascular lesion

### Business Goals:

The primary objective is to construct a multiclass classification model using a custom convolutional neural network (CNN) in TensorFlow.

### Business Risks:

The primary risk associated with this project is the potential for incorrect skin cancer classification.

## Project Pipeline
- Data Acquisition/Data Understanding: Specify file paths for training and testing images.
- Dataset Preparation: Create training and validation datasets from the training directory, resizing images to 180x180 pixels and using a batch size of 32.
- Dataset Visualization: Develop code to visualize representative samples from all nine disease classes.
- Model Building & Training (Initial):
  - Design a CNN model capable of accurately classifying the nine disease classes. Normalize pixel values to the range of 0 to 1.
  - Select an appropriate optimizer and loss function for model training.
  - Train the model for approximately 20 epochs.
  - Document findings post-training, checking for signs of model overfitting or underfitting.
- Addressing Data Augmentation: Implement data augmentation techniques to mitigate underfitting or overfitting.
- Model Building & Training (Augmented Data):
  - Construct a CNN model that can accurately classify the nine disease classes. Normalize pixel values between 0 and 1.
  - Choose a suitable optimizer and loss function.
  - Train the model for around 20 epochs.
  - Summarize findings after training, examining whether previous issues were resolved.
- Class Distribution Analysis: Analyze the current class distribution in the training dataset.
  - Identify the class with the fewest samples.
  - Determine which classes are overrepresented in terms of the proportionate number of samples.
- Addressing Class Imbalances: Correct class imbalances in the training dataset using the Augmentor library.
- Model Building & Training (Balanced Data):
  - Develop a CNN model capable of accurately classifying the nine disease classes. Normalize pixel values to the range of 0 to 1.
  - Choose an appropriate optimizer and loss function for model training.
  - Train the model for approximately 30 epochs.
  - Summarize findings after training, assessing whether the identified issues have been resolved.

## Technologies Used
- pandas - 1.3.4
- numpy - 1.20.3
- matplotlib - 3.4.3
- seaborn - 0.11.2
- plotly - 5.8.0
- scikit-learn - 1.1.2
- statsmodels - 0.13.2
- tensorflow - 2.11.0

## Acknowledgments
- This project was conducted as part of an advanced online course.

## Contact
Created by [@shansalance] - feel free to contact me!

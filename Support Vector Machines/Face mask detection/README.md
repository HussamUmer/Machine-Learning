# 😷 Face Mask Detection using Support Vector Machine (SVM)

This project focuses on building a binary image classifier to detect whether a person is wearing a mask or
not using a Support Vector Machine (SVM) model. We used the "Face Mask Detection ~12K Images Dataset", which
contains over 12,000 labeled images, organized into train, validation, and test directories.

---------------------------------------------------------------------------------------------------------------

## 🧠 Objective

The goal was to train a machine learning model that can automatically classify images of people as:
    1. With Mask 😷
    2. Without Mask 😐

This task is especially relevant in public safety contexts like health monitoring during pandemics.

-----------------------------------------------------------------------------------------------------------------

## 📁 Dataset Overview

The dataset contains 12,000+ images distributed across 3 directories:
  1. train/
  2. validation/
  3. test/

Each directory includes two subfolders:
  1. WithMask/
  2. WithoutMask/

The dataset is balanced, with approximately the same number of images for both classes.

🧾 Note: Due to the large size of the dataset, model training can be computationally intensive and time-consuming,
especially without a GPU.

Dataset Link:[Face Mask Detection 12K Images Dataset](https://www.kaggle.com/datasets/ashishjangra27/face-mask-12k-images-dataset)

---------------------------------------------------------------------------------------------------------------------

## 🛠️ Project Workflow

1. Data Loading & Preprocessing
--------------------------------
    # Loaded the image data from folders using ImageDataGenerator.
    # Resized all images to 128x128 pixels for consistency.
    # Normalized pixel values between 0 and 1.

2. Exploratory Data Analysis (EDA)
-----------------------------------
    # Displayed a few sample images from each class.
    # Observed balanced class distribution.

3. Model Training
------------------
    # Used an SVM classifier with an RBF kernel (nonlinear decision boundary).
    # Converted images to flattened vectors (after resizing).
    # Trained the model on the training set.
    # Evaluated using the validation set.

4. Model Evaluation
--------------------
    # Calculated accuracy, precision, recall, and F1-score.
    # Displayed confusion matrix to analyze class-wise performance.
    # Made predictions on the unseen test set and visualized results.

-------------------------------------------------------------------------------------------------------------------

✅ Results
===========
📊 Evaluation on Validation Set:
---------------------------------

     ✅ Accuracy: 91.25%

The model performs very well on both classes, with slightly better recall for "Without Mask" and better precision
for "With Mask".

------------------------------------------------------------------------------------------------------------------------

🧪 Final Predictions
======================
We also ran predictions on the test set and displayed a few examples with predicted labels, which matched well
visually with the actual appearance of masks or no masks.

------------------------------------------------------------------------------------------------------------------------

💾 Model Saving
================
We saved the trained SVM model using joblib, so it can be reused later without retraining:

   "joblib.dump(model, 'svm_mask_classifier.pkl')"

-------------------------------------------------------------------------------------------------------------------------

❗ Challenges
=============
    1. The dataset size made it slower to preprocess and train the model.
    2. SVMs aren’t GPU-accelerated, so training on high-resolution images or large datasets can take time.
    3. Flattening images may lead to loss of spatial relationships compared to using CNNs.

--------------------------------------------------------------------------------------------------------------------------

💡 Future Improvements
=======================
     1. Switch to a Convolutional Neural Network (CNN) for better performance and efficiency on images.
     2. Add data augmentation for better generalization.
     3. Deploy the model in a real-time application using OpenCV or a web interface.

--------------------------------------------------------------------------------------------------------------------------

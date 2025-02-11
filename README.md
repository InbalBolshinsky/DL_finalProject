# 🩺  DL_finalProject - Lung Cancer Classification using CNNs and Transfer Learning
## - A Deep Learning Approach for Multi-Class Lung Cancer Detection -
## This project was done in the "Deep Learning" course.

## 📌 Project Overview
This project classifies lung cancer images into three categories:

Benign Cases
Malignant Cases
Normal Cases

# The models used include:
✅ Convolutional Neural Networks (CNNs) trained from scratch
✅ Transfer Learning Models (VGG16, ResNet, EfficientNet) with fine-tuning

This project explores data augmentation, class balancing techniques, hyperparameter tuning, and a detailed comparison between CNNs and Transfer Learning models to achieve high accuracy.

## 🔹Dataset
# The dataset used in this project is The IQ-OTHNCCD Lung Cancer Dataset. Ensure that images are stored in the correct folder:
📂 dataset/
    ├── Benign/
    ├── Malignant/
    ├── Normal/

## 🛠️ Methodology

# 1️⃣ Data Preprocessing & Augmentation
Converted grayscale images to 3-channel format (for transfer learning models).
Applied data augmentation (rotation, zoom, flip) to increase dataset diversity.
Computed class weights to counteract class imbalance.

# 2️⃣ Model Training & Hyperparameter Tuning
CNN Model (Trained from Scratch)
Built a Convolutional Neural Network (CNN) using the Functional API.
Applied early stopping to prevent overfitting.
Used class weights to improve model performance on minority classes.
Hyperparameter Tuning
Used KerasTuner’s Hyperband to optimize:
Number of filters per layer
Dense layer units
Dropout rate
Learning rate
Transfer Learning Model (VGG16, ResNet, EfficientNet)
Used VGG16/ResNet/EfficientNet pretrained models with frozen layers.
Fine-tuned the top layers for better feature extraction.

# 3️⃣ Model Evaluation & Performance Comparison
The models were evaluated using:
Precision, Recall, F1-Score (to assess class-wise performance).
Confusion Matrices (to visualize classification accuracy per class).

# 📊 Model Performance Comparison

![DL_finalProject_accuracy](https://github.com/user-attachments/assets/f48fceb1-e274-4b14-80bf-873c287c2c7b)

![DL_finalProject_loss](https://github.com/user-attachments/assets/4a32a3ce-858b-478a-957f-fd01eb8cc129)

##📌 Key Observations:
# ✅ Data augmentation & class weights improved recall on minority classes.
# ✅ Hyperparameter tuning significantly improved CNN performance.
# ✅ Transfer learning (VGG16) achieved excellent accuracy but is computationally expensive.



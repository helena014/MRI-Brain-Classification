# MRI-Brain-Classification
Brain MRI Image Classification using Deep Learning and ResNet18

📌 Project Overview

This project uses Deep Learning to classify brain MRI images into four Alzheimer's disease categories based on their image patterns.

A ResNet-18 Convolutional Neural Network (CNN), using transfer learning with pretrained ImageNet weights, was implemented using PyTorch. The model was trained on Google Colab with GPU acceleration.

🎯 Problem Statement

Alzheimer's disease is a progressive neurological disorder that affects memory and cognitive abilities. This project explores the use of deep learning and MRI image classification to identify different stages of dementia from brain MRI scans.

📂 Dataset

Source: Alzheimer's Dataset – Kaggle

Dataset Structure: Training and testing folders.

Number of Classes: 4

Classification Categories

MildDemented

ModerateDemented

NonDemented

VeryMildDemented

The dataset was downloaded directly from Kaggle using the kagglehub library.

🛠️ Technologies Used

Python

PyTorch

Torchvision

KaggleHub

NumPy

Google Colab (GPU)

⚙️ Project Workflow

Dataset Acquisition: Downloaded the Alzheimer's MRI dataset using KaggleHub.

Image Preprocessing: Resized images to 224 × 224 pixels, applied random horizontal flipping for training augmentation, converted images to tensors, and normalized them using ImageNet mean and standard deviation.

Data Loading: Used PyTorch ImageFolder and DataLoader with a batch size of 32.

Model Architecture: Implemented pretrained ResNet-18 and modified its final fully connected layer to classify four categories.

Model Training: Trained the model for 5 epochs using Cross Entropy Loss and the Adam optimizer with a learning rate of 0.0001.

Model Evaluation: Evaluated the trained model on the test dataset.

Model Saving: Saved the trained model weights as alzheimer_mri_resnet18.pth.

📊 Results

Final Test Accuracy: 98.70%

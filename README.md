# 🐾 Denoising Images with a Convolutional Autoencoder
This project demonstrates how to build and train a Convolutional Denoising Autoencoder (CDAE) using TensorFlow and Keras to clean noisy images from the Oxford-IIIT Pet Dataset.

## 📌 Project Description
We explore the use of deep learning to remove noise from images by training a CDAE. The autoencoder learns to reconstruct clean images from their noisy counterparts. This notebook includes:

 - Loading and preprocessing the Oxford-IIIT Pet Dataset
 - Adding Gaussian noise to the images
 - Building a convolutional autoencoder using TensorFlow/Keras
 - Training and evaluating the denoising performance
 - Visualizing results and model performance

## 🗂 Dataset
 - Oxford-IIIT Pet Dataset: A collection of 37 pet categories with roughly 200 images per class.
 - Only the raw image files were used in this task, with no labels.

## 🧠 Model Architecture
 - Encoder: 2 convolutional layers + max pooling
 - Decoder: 2 transposed convolutional layers + upsampling
 - Loss Function: Mean Squared Error (MSE)
 - Optimizer: Adam

## 🧪 Experiments
 - Images were corrupted using Gaussian noise
 - Trained model for 20 epochs with batch size 32
 - Compared original, noisy, and denoised images for evaluation

## 📊 Results
 - Visualization of training/validation loss over epochs
 - Side-by-side comparison of:
   - Noisy input
   - Ground truth
   - Autoencoder output

## 📦 Dependencies
 - Python 3.x
 - TensorFlow
 - NumPy
 - OpenCV
 - Matplotlib
 - scikit-learn

## 🚀 Usage
 - Download the Oxford-IIIT Pet Dataset from Kaggle or your preferred source.
 - Update the data_path in the notebook to point to the image folder.
 - Run the notebook to train and visualize the results.

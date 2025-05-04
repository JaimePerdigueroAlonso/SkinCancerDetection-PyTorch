# Skin Cancer Detection using Deep Learning

## 1. Introduction

This project implements a deep learning model for skin cancer detection, classifying images as either benign or malignant. It uses the PyTorch library to build and train a convolutional neural network (CNN) based on the ResNet18 architecture. The dataset used is the "Melanoma Skin Cancer Dataset of 10000 images" available on Kaggle.

## 2. Project Structure

The project is divided into the following main stages:

* **Library Imports:** Necessary libraries for data handling, image processing, model building, training, and evaluation.
* **Dataset Download:** Downloading the dataset from Kaggle using `kagglehub`.
* **Data Loading and Preprocessing:** Loading images, resizing, converting to numpy arrays, and splitting into training and testing sets.
* **Data Visualization:** Displaying sample images from the dataset.
* **Dataset and DataLoader Creation:** Creating PyTorch Datasets and DataLoaders for efficient data handling.
* **Model Definition:** Loading a pre-trained ResNet18 model and customizing its final layer.
* **Loss Function and Optimizer Definition:** Defining the loss function and optimizer for training.
* **Model Training:** Training the model over multiple epochs and tracking performance.
* **Model Evaluation:** Evaluating the trained model on the test set and visualizing the confusion matrix.
* **User Photo Upload and Prediction (Extension):** Guidance on how to add functionality for users to upload images and receive predictions.

## 3. How to Run the Project

1.  **Environment:** Google Colab is recommended.
2.  **Dependencies:** Ensure you have the following libraries:
    * `os`
    * `PIL (Pillow)`
    * `numpy`
    * `torch`
    * `torchvision`
    * `matplotlib`
    * `scikit-learn`
    * `kagglehub`
3.  **Execution:** Run the cells in the Colab notebook sequentially.

## 4. User Photo Upload and Prediction (Extension)
This section outlines how to extend the project to allow users to upload their own images for prediction.

If you are running this notebook in Google Colab and want to test it with your own images, follow these steps:

1.  **Upload Images:** Upload your image files directly to the `/content/` directory in the Colab environment. You can do this by clicking the folder icon in the left sidebar, then the upload icon.

2.  **Rename Files (If Necessary):** Ensure that the file names in your code match the names of the files you've uploaded.  For example, if the original code references files named `"bueno.jpg"`, `"bueno1.jpg"`, `"malo.jpg"`, and `"malo1.jpg"`, and your uploaded files have different names (e.g., `"my_skin_image1.png"`, `"test_photo.jpeg"`), you **must** change the file names in the code to reflect your actual file names.

## 5.  Dataset Availability

For your convenience, we have included the necessary datasets in a separate section of the GitHub repository.

* **Melanoma Dataset:** The "Melanoma Skin Cancer Dataset of 10000 images" from Kaggle is provided in the `melanoma_dataset/` directory.
* **Test Images:** The four test images (e.g., `"bueno.jpg"`, `"bueno1.jpg"`, `"malo.jpg"`, `"malo1.jpg"`) are located in the `test_images/` directory.

You can use these directories directly if you prefer not to download the data within the Colab notebook. However, note that using the Kaggle download within the notebook ensures you're using the exact version of the dataset used during development.

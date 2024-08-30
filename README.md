# Traffic Sign Recognition Using CNN

This project implements a Traffic Sign Recognition system using Convolutional Neural Networks (CNN). The system is designed to classify various traffic signs with high accuracy, making it a crucial tool for autonomous driving and advanced driver assistance systems.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Web Application](#web-application)
- [Real-time Recognition](#real-time-recognition)
- [Conclusion](#conclusion)

## Introduction

Traffic Sign Recognition is a key component in the development of autonomous vehicles. This project focuses on creating a CNN model capable of accurately recognizing and classifying traffic signs from images. The system can be integrated into various applications, including real-time recognition in vehicles.

## Project Structure

- `data/`: Contains the dataset used for training and testing.
- `notebooks/`: Jupyter Notebooks used for data exploration, model development, and training.
- `models/`: Saved models and checkpoints.
- `app/`: Flask web application for traffic sign recognition.
- `real_time/`: Scripts for real-time traffic sign recognition using a webcam.
- `scripts/`: Utility scripts for data preprocessing, training, and evaluation.
- `README.md`: Project documentation.

## Dataset

The project uses a dataset of traffic signs, which includes various classes of signs captured under different conditions. The dataset is pre-split into training, validation, and test sets.

## Data Preprocessing

Before feeding the data into the CNN, several preprocessing steps are applied:
- **Normalization**: Scaling pixel values to the range [0, 1].
- **Augmentation**: Applying transformations like rotation, scaling, and flipping to increase data diversity.
- **Resizing**: Ensuring all images are of uniform size.

## Model Architecture

The CNN model is designed with multiple convolutional layers followed by pooling layers, fully connected layers, and a softmax output layer. The architecture is optimized for high accuracy in traffic sign classification.

## Training

The model is trained using TensorFlow, with a focus on minimizing categorical cross-entropy loss. Various techniques like dropout and batch normalization are used to prevent overfitting.

## Evaluation

The model's performance is evaluated using accuracy, precision, recall, and F1-score metrics on the test set. Confusion matrices and ROC curves are also generated to analyze the results.

## Web Application

A simple Flask web application is included, allowing users to upload images and receive predictions on the traffic sign class.

## Real-time Recognition

An optional real-time recognition script is provided, which uses a webcam to detect and classify traffic signs in real time.

## Conclusion

This project demonstrates the potential of CNNs in traffic sign recognition, contributing to safer autonomous driving systems. The next steps include improving model accuracy and deploying the system in real-world applications.


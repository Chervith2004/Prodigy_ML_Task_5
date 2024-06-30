# Prodigy_ML_Task_5

Linkedin post link:https://www.linkedin.com/posts/gottipati-2004-chervith_machinelearning-prodigyinfotech-activity-7213158964170039297-q9_j?utm_source=share&utm_medium=member_desktop

Overview: This repository contains a project for classifying food images using a DenseNet-201 model. The project includes data preprocessing, model training, and evaluation. The dataset used is the Food-101 dataset, which contains images of 101 different food categories.

Dataset: The Food-101 dataset is used in this project. It contains 101,000 images of food items, with 1,000 images per class. The dataset is divided into training and testing sets.

Project Structure: data/: Contains the Food-101 dataset. notebooks/: Jupyter notebooks for exploratory data analysis and model training. models/: Contains the trained model. scripts/: Python scripts for data preprocessing, model training, and evaluation.

Data Preprocessing: The dataset is preprocessed by reading the image paths, separating the labels and image indices, and storing them in a pandas DataFrame. The data is then shuffled for randomness.

Model: A DenseNet-201 model pretrained on ImageNet is used. The final layer is modified to classify 101 food categories. The model parameters are frozen to utilize the pretrained weights, except for the classifier layer which is trained on the Food-101 dataset.

Training: The training process involves: Data augmentation using random rotations, crops, and horizontal flips. Training the model using cross-entropy loss and the Adam optimizer. Evaluating the model on the test set after each epoch.

Evaluation: The model's performance is evaluated using accuracy metrics on the test set. The best model based on the test accuracy is saved.

Usage: Train the model Evaluate the model Visualize results and predictions using the provided Jupyter notebooks.

Results: The model achieves an accuracy of over 91% on the test set after training for 3 epochs.


Facial Recognition with SVM, Random Forest, and CNN

This project demonstrates a facial recognition task using the Labeled Faces in the Wild (LFW) dataset. It implements and compares three different machine learning models: Support Vector Machine (SVM), Random Forest, and a Convolutional Neural Network (CNN) to classify individuals based on their facial features.

Project Overview

The goal of this project is to showcase the application of various machine learning algorithms for multi-class facial classification. The LFW dataset, a public benchmark for facial recognition, is used to train and evaluate the models. The project includes data loading, preprocessing, model training, and a comprehensive evaluation of each model's performance using accuracy, confusion matrices, and Receiver Operating Characteristic (ROC) curves.

Features

Dataset Loading & Preprocessing: Loads the LFW dataset, normalizes features using MinMaxScaler, and encodes labels.
Data Splitting: Divides the dataset into training and testing sets with stratification to maintain class distribution.
Model Implementations:

Support Vector Machine (SVM): Trained with a radial basis function (RBF) kernel and StandardScaler in a pipeline.
Random Forest Classifier: An ensemble learning method.
Convolutional Neural Network (CNN): A deep learning model designed for image classification, built with tensorflow.keras.
Model Evaluation:

Calculates and displays classification accuracy for each model.
Generates and visualizes Confusion Matrices to show per-class performance.
Plots multi-class ROC curves with AUC scores for each class to assess model discriminative power.
Performance Comparison: Provides a bar chart comparing the accuracy of all three models.
Setup and Installation
To run this notebook, you'll need to install the following Python libraries. You can install them using pip:

pip install scikit-learn numpy tensorflow matplotlib
How to Run
Clone the Repository (if applicable) or Open in Colab: If you have the .ipynb file, open it in Google Colab.
Execute Cells: Run all the cells in the notebook sequentially.
The first few cells will load and preprocess the LFW dataset.
Subsequent cells will train the SVM, Random Forest, and CNN models, respectively.
Evaluation functions will then be called to display metrics and plots for each model.
Finally, a bar chart will compare the overall accuracies.
Results and Findings
After training and evaluating the models on the LFW dataset (with min_faces_per_person=70 and resize=0.4), the following accuracies were observed:

SVM: 0.7795
Random Forest: 0.6273
CNN: 0.5870

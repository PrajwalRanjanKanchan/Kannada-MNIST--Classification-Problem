# Kannada-MNIST--Classification-Problem

## Problem Statement
Problem Statement: This is an extension of clasic MNIST classification problem. Instead of using
Hindu numerals, lets use a recently-released dataset of Kannada digits. This is a 10 Class classification
problem.
Kannada is a language spoken predominantly by people of Karnataka in southwestern India. The
language has roughly 45 million native speakers and is written using the Kannada script. https:
//en.wikipedia.org/wiki/Kannada
Dataset can be downloaded from the link : https://www.kaggle.com/datasets/higgstachyon/
kannada-mnist.

All details of the dataset curation has been captured in the paper titled: Prabhu, Vinay Uday. "Kannada-
MNIST: A new handwritten digits dataset for the Kannada language."https://arxiv.org/abs/1908.01242

## Libraries Used
1. numpy
2. scikit-learn
3. matplotlib

## Approach

1. Data Collection and Preprocessing:
   - Extracting the dataset from the provided npz file, containing 60,000 training and 10,000 test images, each with a size of 28x28 pixels.
   - Normalizing the pixel values to a range of 0 to 1 and reshape the images for further processing.

2. Dimensionality Reduction with PCA:
   - Performing PCA (Principal Component Analysis) to reduce the image dimensions from 28x28 to a compact 10-dimensional representation.
   - Retaining the most important features while reducing computational complexity.

3. Model Selection and Training:
   - Implementing five powerful classification models: Decision Trees, Random Forest, Naive Bayes, K-NN Classifier, and SVM.
   - Train each model using the transformed training data in 10 dimensions.

4. Model Evaluation and Metrics:
   - Evaluating the performance of each model using essential metrics like Precision, Recall, and F1-Score.
   - Generating Confusion Matrix to analyze the accuracy of predictions for all classes.
   - Visualizing the Receiver Operating Characteristic (RoC) curve to gauge model performance.

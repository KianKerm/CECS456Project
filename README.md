# CECS456Project



##Project Overview

This project implements and compares two Convolutional Neural Network (CNN) models for multi-class medical image classification using the Medical MNIST dataset. The dataset contains 64×64 images across six categories: AbdomenCT, BreastMRI, CXR, ChestCT, Hand, and HeadCT.

The workflow includes:

Loading and preprocessing images (resizing to 64×64 and normalizing pixel values to [0, 1])

Detecting and removing duplicate images 

Performing basic class balance analysis

Training and evaluating two CNN architectures:

Model 1: A baseline 3-block CNN with MaxPooling and Dropout, followed by a Dense classifier head

Model 2: A modified CNN incorporating Batch Normalization and Global Average Pooling to improve training stability and reduce parameter count

Model performance is evaluated using:

Training/validation accuracy and loss curves

Test accuracy and AUC

Confusion matrices

Qualitative inspection of misclassified examples

Both models achieved very strong performance, with Model 2 showing slightly better generalization and fewer test-set errors.


# Eigenfaces-Based Face Recognition System

This project implements a classical facial recognition system using the Eigenfaces approach based on Principal Component Analysis (PCA). The objective is to demonstrate both the mathematical foundations of the Eigenfaces algorithm and its application in a full-scale face recognition system without using deep learning techniques.

## Project Structure

This repository contains two main implementations:

### 1. Mathematical Demonstration
A from-scratch implementation using a small synthetically generated face dataset to verify the mathematical working of PCA, eigenface computation, projection into eigenface space, reconstruction, and distance-based face matching. This part focuses on understanding and visualizing the core concepts behind the Eigenfaces method.

File:
- `code/Eigenfaces_Face_Recognition_Full_Math_&_Visualization.ipynb`

### 2. System-Level Implementation
An extended implementation applied to the AT&T (ORL) Face Dataset to demonstrate full facial recognition performance on multiple subjects. This part evaluates recognition accuracy, variance retention, and classification behavior using PCA and K-Nearest Neighbors (KNN).

File:
- `code/eigenfaces_orl_system.ipynb`

## Methodology
- Convert face images to grayscale and resize them to a consistent resolution
- Represent images as high-dimensional vectors
- Compute the mean face and subtract it from all images
- Apply Principal Component Analysis (PCA) to extract eigenfaces
- Project images into a reduced-dimensional eigenface space
- Perform face recognition using Euclidean distance and KNN
- Analyze reconstruction quality and recognition accuracy

## Datasets
- **Synthetic Face Dataset**: AI-generated facial images used for mathematical demonstration and visualization
- **AT&T (ORL) Face Dataset**: A standard benchmark dataset used for system-level facial recognition and evaluation

## Results
- Achieved approximately **98–100% recognition accuracy** using around **35 eigenfaces**
- Retained nearly **99% variance** in the reduced PCA space
- Demonstrated effective dimensionality reduction and accurate face reconstruction under controlled conditions

## Tools and Technologies
Python, NumPy, Matplotlib, Principal Component Analysis (PCA), K-Nearest Neighbors (KNN)

## Notes
Synthetic face images are used strictly for academic and non-commercial demonstration purposes. The system-level implementation is adapted and extended from publicly available open-source references for educational use.

## References
- Turk, M., and Pentland, A. (1991). *Eigenfaces for Recognition*
- AT&T (ORL) Face Dataset


# Neural Networks Project Collection

## Overview
This repository contains implementations of various neural network projects, each utilizing a different type of neural network architecture. The projects cover a range of tasks, from image generation to text classification, demonstrating the versatility of neural networks in solving diverse problems.

---

## Project List

### 1. Variational Autoencoder (VAE): Traffic Sign Generation
- **Task:** Generate synthetic images of traffic signs.
- **Dataset:** Provided as `trafic_32.zip` (similar structure to ImageFolder).
- **Output:** 1,000 generated images saved as a PyTorch tensor.
- **Evaluation:** Frechet Inception Distance (FID) metric.

### 2. Long Short-Term Memory (LSTM): Composer Prediction
- **Task:** Predict the composer of classical music based on chord sequences.
- **Dataset:** Provided in `train.pkl` (training data) and `test_no_target.pkl` (test data).
- **Classes:** Bach, Beethoven, Debussy, Scarlatti, Victoria.
- **Special Requirements:**
  - Use padding or `PackedSequence` for variable-length sequences.
  - Output predictions in a CSV file without headers or indices.

### 3. Feedforward Neural Network (FNN): Housing Price Classification
- **Task:** Classify properties as `cheap`, `average`, or `expensive`.
- **Dataset:** Training data in `train_data.csv` and test data in `test_data.csv`.
- **Output:** CSV with predicted class for each test instance (0: cheap, 1: average, 2: expensive).
- **Special Notes:**
  - Handle class imbalance.
  - Ensure predictions file is correctly formatted with no extra rows or columns.

### 4. Convolutional Neural Network (CNN): Image Classification
- **Task:** Classify images into 50 classes of objects and animals.
- **Dataset:** Training set with subfolders per class and a flat test set.
- **Output:** CSV with filenames and corresponding predicted classes.
- **Special Notes:**
  - Use custom architectures (do not use pretrained models).
  - Include two columns in the predictions CSV: filename and predicted class index.

### 5. BERT: Hotel Review Classification
- **Task:** Predict star ratings (0 to 4) based on hotel reviews.
- **Dataset:** Provided training set.
- **Output:** CSV with predicted ratings for the test set.
- **Special Notes:**
  - Tackle this as a multi-class classification problem.
  - Ensure predictions match the order of test samples.

---


# Word-For-Thought

## Overview

Speech Emotion Recognition (SER) is a key component in human-computer interaction systems, enabling machines to understand and respond to human emotions through speech signals.

This project focuses on developing a deep learning-based audio classification system capable of accurately identifying human emotional states from speech recordings. The model leverages advanced audio feature extraction techniques and Convolutional Neural Networks (CNNs) to classify emotions with high accuracy across benchmark datasets.

---

## Objective

The primary objective of this project is to accurately classify human emotions from speech signals using deep learning techniques.

The system aims to:

- Analyze raw audio recordings and extract meaningful acoustic features.
- Learn emotion-specific speech patterns through a CNN-based architecture.
- Achieve strong generalization across diverse speakers and recording conditions.
- Provide an efficient and scalable framework for speech emotion recognition applications.

---

## Datasets

The model was trained and evaluated on two widely used benchmark datasets:

### 1. RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)
- Professional recordings from multiple actors.
- Contains speech samples expressing different emotions.
- Widely used for speech emotion recognition research.

### 2. CREMA-D (Crowd-Sourced Emotional Multimodal Actors Dataset)
- Contains emotionally rich speech recordings from a diverse set of actors.
- Includes multiple emotional categories with varying intensity levels.
- Provides greater speaker diversity and real-world variability.

---

## Methodology

### 1. Audio Preprocessing

Raw speech recordings were preprocessed to improve feature quality and model performance.

Steps included:

- Loading and normalizing audio signals.
- Resampling audio to a consistent sampling rate.
- Noise reduction and signal standardization.
- Feature extraction for deep learning input generation.

---

### 2. Feature Extraction

To capture the most informative characteristics of speech signals, Mel-Frequency Cepstral Coefficients (MFCCs) were extracted from each audio sample.

MFCCs are widely used in speech processing because they:

- Mimic human auditory perception.
- Capture timbral and spectral characteristics of speech.
- Reduce dimensionality while preserving critical information.
- Improve emotion classification performance.

Extracted MFCC features were converted into structured representations suitable for CNN training.

---

### 3. Deep Learning Architecture

A Convolutional Neural Network (CNN) was designed specifically for emotion recognition from audio features.

#### Architecture Highlights

- Multiple convolutional layers for hierarchical feature extraction.
- Activation functions for non-linear learning.
- Pooling layers for dimensionality reduction.
- Fully connected layers for emotion classification.
- Regularization techniques to prevent overfitting.

The CNN learns both low-level acoustic patterns and high-level emotional characteristics from speech data.

---

### 4. Hyperparameter Optimization

Extensive experimentation was performed to improve model performance.

Optimized parameters included:

- Learning rate
- Batch size
- Number of convolutional filters
- Kernel sizes
- Dropout rates
- Training epochs

The optimization process improved both model accuracy and inference efficiency while maintaining strong generalization on unseen data.

---

## Results

### Performance Metrics

| Metric | Value |
|----------|---------|
| Test Accuracy | **88%** |
| Datasets | RAVDESS + CREMA-D |
| Model Type | CNN |
| Features | MFCC |



## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Librosa
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## Project Workflow

```text
Audio Dataset
      │
      ▼
Preprocessing
      │
      ▼
MFCC Feature Extraction
      │
      ▼
Feature Normalization
      │
      ▼
CNN Training
      │
      ▼
Hyperparameter Tuning
      │
      ▼
Emotion Classification
      │
      ▼
Performance Evaluation

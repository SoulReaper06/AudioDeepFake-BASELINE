# DeepFake Audio Detection System - Baseline

## Overview

This project focuses on the development of a DeepFake audio detection system using the ASVSpoof 2019 dataset. The goal is to identify manipulated or fake audio recordings, commonly referred to as DeepFake audio, and distinguish them from genuine recordings.

## Dataset

The ASVSpoof 2019 dataset was utilized for training and evaluation. This dataset consists of a variety of spoofed and bonafide audio samples, providing a comprehensive set of challenges for training robust models.

- **Size:** The dataset contains a total of X samples, with Y% dedicated to training, Z% for validation, and W% for testing.

- **Classes:** The two main classes are "bonafide" representing genuine audio and "spoofed" representing manipulated or fake audio.

## Model Architecture

The DeepFake audio detection system employs a deep neural network architecture, specifically designed for audio classification tasks. The model architecture includes:

- **Input Layer:** LFCC (Logarithmic Frequency Cepstral Coefficients) representations of audio signals were used as input features.

- **Convolutional Layers:** Multiple convolutional layers to capture hierarchical features from the input spectrograms.

- **Recurrent Layers:** Bidirectional LSTM layers to capture temporal dependencies in the audio sequences.

- **Dense Layers:** Fully connected layers for final classification.

- **Output Layer:** Sigmoid activation to predict the probability of a sample being spoofed.

## Training

The model was trained using the ASVSpoof 2019 training set with the following training parameters:

- **Optimizer:** Adam
- **Learning Rate:** 0.001
- **Loss Function:** Binary Crossentropy
- **Batch Size:** 32
- **Epochs:** 50

## Evaluation Results

The model's performance was evaluated on the ASVSpoof 2019 evaluation set. The evaluation results are as follows:

```markdown
| Metric      | Value   |
|-------------|---------|
| Accuracy    | 0.92    |
| Precision   | 0.90    |
| Recall      | 0.94    |
| F1 Score    | 0.92    |

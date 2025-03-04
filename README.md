

# Speech Emotion Recognition using CNN

This project aims to build a **Speech Emotion Recognition (SER)** system using **Convolutional Neural Networks (CNNs)**. The system classifies various emotions like **Neutral, Happy, Angry, Sad, Fear, Disgust, Surprise** from speech signals, providing a solution for various applications such as virtual assistants, mental health monitoring, and human-computer interaction.

## Table of Contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Installation](#installation)
4. [Model Architecture:](#model-architecture)
5. [Datasets Used](#datasets-used)
6. [Evaluation](#evaluation)
7. [Contributing](#contributing)


## Introduction

Speech Emotion Recognition is a critical task in human-computer interaction, enabling machines to understand and react to emotions expressed in speech. This project uses **Convolutional Neural Networks (CNNs)** for emotion classification based on **spectrogram representations** of audio signals.

## Project Overview

The project consists of the following components:
- **Data Preprocessing**: Conversion of audio signals into spectrograms using **Librosa**.
- **Feature Extraction**: Extraction of key features such as **Zero Crossing Rate (ZCR)**, **Mel-Frequency Cepstral Coefficients (MFCC)**, and **Root Mean Square Error (RMSE)** to help the model learn emotional patterns.
- **Model Architecture**: A deep **CNN-based architecture** to extract hierarchical features from spectrograms and classify emotions.
- **Real-time Prediction Interface**: A user-friendly web interface built with **Streamlit** that allows users to upload speech files and receive real-time emotion predictions.
- **Hyperparameter Tuning**: Extensive experimentation to optimize model performance and achieve state-of-the-art results.

## Installation

To run this project locally, follow these steps:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/nasarinagasunil/Speech_Emotion_Recognition_using_CNN.git
   cd Speech_Emotion_Recognition_using_CNN
   ```

2. **Install Dependencies**
   You can install the required dependencies:
   ```bash
   ```
   - `tensorflow`
   - `librosa`
   - `streamlit`
   - `matplotlib`
   - `seaborn`
   - `numpy`
   - `pandas`

## Model Architecture: 

### **Feature Extraction**:
The model extracts several key audio features to facilitate emotion recognition:

- **Zero Crossing Rate (ZCR)**: Measures the rate at which the signal changes polarity, which is useful for distinguishing between noisy and tonal signals.
- **Mel-Frequency Cepstral Coefficients (MFCC)**: Widely used in speech and audio processing, MFCCs capture the timbral features of an audio signal.
- **Root Mean Square Error (RMSE)**: Represents the energy of the speech signal, which can vary across different emotional states.

These features are extracted from the raw audio signals and used as input for the CNN model.

### **CNN Architecture**:
The core of the model is a **Convolutional Neural Network (CNN)** that learns hierarchical patterns from the spectrograms and extracted features. The architecture consists of:
1. **Input Layer**: Takes spectrogram representations of audio signals.
2. **Convolutional Layers**: Multiple convolutional layers to extract hierarchical features from spectrograms.
3. **Pooling Layers**: Max pooling layers for dimensionality reduction and feature extraction.
4. **Fully Connected Layers**: Dense layers for final emotion classification.
5. **Output Layer**: Softmax output for multi-class classification of emotions.

The model has been optimized through extensive hyperparameter tuning to achieve state-of-the-art performance.

## Datasets Used

The following datasets were used to train and evaluate the model:

- **RAVDESS**
- **TESS**
- **CREMA**
- **SAVEE**
  
These datasets are preprocessed to extract features and generate labels corresponding to emotional classes.
### Emotion Classes

   - Neutral
   - Happy
   - Sad
   - Angry
   - Fear
   - Disgust
   - Surprise

## Evaluation

The model was evaluated on benchmark datasets, achieving high accuracy in emotion classification. The following performance metrics were considered:
- **Accuracy**: 80%
- **Loss**: 40%


## Contributing

Contributions to this project are welcome! Please follow these steps to contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.


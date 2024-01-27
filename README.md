# Iqraa w Irtaqi Ai Model

This code aims to build a convolutional neural network (CNN) model capable of recognizing Quran speech audio and converting it into text with correction.

Key Features:

Audio Preprocessing:
Extracts mel-frequency cepstral coefficients (MFCCs) from audio files.
Applies harmonic effects to enhance audio signals.
Text Preprocessing:
Converts text labels into numerical sequences for model training.
CNN Architecture:
Employs convolutional layers with max pooling and dropout for feature extraction.
Uses dense layers for final classification.
Training:
Compiles the model with Adam optimizer and categorical crossentropy loss.
Trains the model on audio and text data, monitoring validation loss.
Incorporates early stopping and learning rate reduction to prevent overfitting.
Evaluation:
Assesses model performance on a test set using accuracy metrics.
Generates predictions for audio samples in the test set.
Key Files and Directories:

config/model.conf: Configuration file for model settings.
generatedmodel/: Directory to store trained models.
testing/: Directory containing audio files for testing.
Dependencies:

Python 3.x
TensorFlow
Keras
Librosa
NumPy
Pandas
Matplotlib
Instructions for Use:

Install required libraries: pip install -r requirements.txt
Prepare audio and text data for training and testing.
Adjust configuration settings in config/model.conf if needed.
Run the code to train and evaluate the model.
Additional Notes:

The code currently uses a custom CTC loss function, which is commented out.
The TextTransform class handles text preprocessing.
The cnnlib class provides utility functions for loading and testing the model.

# Image Captioning Project

## Project Description

This project implements an image captioning system that generates textual descriptions for images using a deep learning approach. The system leverages a pre-trained VGG16 model for feature extraction and an LSTM-based sequence model for generating captions. The pipeline includes data preprocessing to clean and tokenize captions, feature extraction from images, and model training to predict captions. Model performance is evaluated using BLEU scores, which measure the quality of generated captions against reference descriptions. This project showcases the application of deep learning techniques in generating descriptive text for visual content.

## Project Structure

- **Data Preparation**
  - Loads and preprocesses image data and corresponding captions from the Flickr8k dataset.
  - Cleans and tokenizes text data, extracts image features using VGG16.

- **Model Construction**
  - Defines and compiles a combined model with an image feature extractor (VGG16) and a sequence model (LSTM).
  - The model predicts captions based on image features and input text sequences.

- **Training**
  - Trains the model using the prepared training dataset and evaluates it on a validation set.
  - Visualizes training and validation loss over epochs.

- **Evaluation**
  - Generates captions for test images and evaluates the results using BLEU scores.
  - Plots examples of generated captions, highlighting both high and low-quality predictions.

## Requirements

- Python 3.x
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- NLTK
- ProgressBar

## Installation

Install the required packages using pip:

```bash
pip install tensorflow keras numpy pandas matplotlib nltk progressbar

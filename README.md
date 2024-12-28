# TweetStance 

This repository contains the code for a stance detection project, which aims to identify the stance or sentiment expressed in text towards a target entity. The model classifies text as either supporting, opposing, or neutral towards a specific target, a task that can be useful for a variety of applications, including social media analysis, opinion mining, and information retrieval.

## Project Overview

The goal of this project is to build a machine learning model that can predict the stance of a given text towards a target. The project uses a dataset of text samples and applies natural language processing (NLP) techniques to train the model.

## Features

- **Stance Classification**: Classifies text into three categories — Support, Against, or Neutral.
- **Text Preprocessing**: Includes tokenization, stopword removal, and text normalization.
- **Model Implementation**: Utilizes popular machine learning models and techniques for stance detection.

## Dataset

The dataset used for training and evaluation contains labeled text samples, each with a corresponding stance label. You can find the dataset in the `/data` directory or refer to the original source (if applicable).

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ragini-kalvade/TweetStance
2. Navigate into the project directory:
      cd stance-detection
3. Install the required dependencies:
      pip install -r requirements.txt

## Usage

Data Preparation: Preprocess the dataset using the provided scripts to clean and format the text.

Training the Model: Use the training script to train the model on the preprocessed data:
    python train_model.py

Making Predictions: Use the trained model to classify new text samples:    
    python predict.py --text "Your text here"
    Example : Given a sample text:
      text: I love this new policy and fully support it!
      The model would classify it as: Support

Evaluation: The model's performance is evaluated using standard metrics such as accuracy, precision, recall, and F1 score. The evaluation script is available for assessing the results on the validation/test dataset.
    python evaluate.py


## Directory Structure

/stance-detection
│
├── data/                  # Dataset files
├── models/                # Saved models
├── notebooks/             # Jupyter notebooks for exploration
├── src/                   # Source code for preprocessing, training, and evaluation
│   ├── preprocess.py      # Data preprocessing script
│   ├── train_model.py     # Script to train the stance detection model
│   ├── predict.py         # Script to make predictions
│   ├── evaluate.py        # Script to evaluate the model
└── requirements.txt       # Python dependencies

# AI-Based Microscopy Image Classification

## Project Overview
This repository contains an AI-based classification model for microscopy images, specifically targeting the classification of nine commonly misidentified cell lines. The project utilizes deep learning techniques with transfer learning on the Xception model to improve classification accuracy. 

This project was developed as part of my AI Master's studies. Please note that this project is still in progress, and improvements will be made over time.

## Features

Preprocessing & Dataset Preparation: Image processing, labeling, and dataset splitting into training, validation, and test sets.

Deep Learning Model: Fine-tuned Xception model for multi-class classification.

Explainable AI (XAI): Model interpretability techniques, including SHAP and LIME, to understand decision-making.

Performance Analysis: Accuracy metrics, confusion matrices, and visual evaluations of the model’s predictions.

# Project Structure
```bash
├── data/
│   ├── images_train/  # Raw microscopy images
│   ├── images/        # Processed images for training
│   ├── classes.csv    # Class labels for images
├── models_xception/   # Trained model checkpoints, model currently only local available
├── main.ipynb         # Data preprocessing and training
├── XAI.ipynb          # Model evaluation and explainability
├── README.md          # Project documentation
```

## Installation

Prerequisites

Ensure you have Python 3.8+ and the following libraries installed:

pip install tensorflow numpy pandas matplotlib seaborn shap lime opencv-python

## Usage

1. Preprocessing & Training

Run the main.ipynb notebook to preprocess images, prepare datasets, and train the model.

2. Model Evaluation & Explainability

Run the XAI.ipynb notebook to evaluate model performance and use explainability techniques such as SHAP and LIME to visualize important regions influencing the classification decisions.

## Results

The model achieves an accuracy of ~87.7% on the validation set.

The confusion matrix highlights misclassifications, particularly among HEK 293, HeLa, and U-2 OS cell lines.

Explainability techniques suggest that the model does not consistently focus on specific distinguishing features of the cells.

## Future Improvements

Data Augmentation: Address class imbalance and improve generalization.

Alternative Architectures: Explore EfficientNet or Vision Transformers.

Improved Explainability: Enhance feature localization to improve trust in model decisions.

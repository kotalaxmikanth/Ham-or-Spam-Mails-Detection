# Spam Email Classification Project

## Overview
This project implements a machine learning-based spam email classifier using Logistic Regression and text classification techniques. The model can distinguish between spam and non-spam (ham) emails with high accuracy.

## Project Structure
- `spam.csv`: Dataset containing email texts and their labels
- `Logistic_Regression.ipynb`: Main Python script for spam classification

## Prerequisites
- Python 3.12+
- Required Libraries:
  - pandas
  - numpy
  - scikit-learn

## Installation
1. Clone the repository
2. Install required dependencies:
```bash
pip install pandas numpy scikit-learn
```

## Dataset
The project uses the `spam.csv` dataset with two primary columns:
- `label`: Classification of email (spam/ham)
- `text`: Email text content

## Methodology
### Data Preprocessing
- Read CSV file with Latin-1 encoding
- Rename columns for clarity
- Remove unnecessary columns

### Feature Extraction
- Use CountVectorizer for text vectorization
- Convert text data into numerical feature matrix

### Model Training
- Algorithm: Logistic Regression
- Training-Test Split: 80% training, 20% testing
- Random State: 42 (for reproducibility)

## Performance Metrics
The model is evaluated using:
- Accuracy Score
- Classification Report (Precision, Recall, F1-Score)

## Model Evaluation
The script generates a classification report showing the model's performance across different metrics.

## Future Improvements
- Experiment with different vectorization techniques
- Try other classification algorithms
- Implement cross-validation
- Handle class imbalance

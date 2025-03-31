# Petition Topic Classifier

This repository contains the code and documentation for **COMP1804 Task 1**, a machine learning project aimed at classifying petition topics based on text data and entity information. The project uses a LinearSVC model with TF-IDF vectorization and achieves high accuracy in predicting petition topics.

## Project Overview
The goal of this project is to classify petition topics from a dataset (`comp1804_coursework_dataset_24-25.csv`) into one of seven categories, such as "education," "health and social care," and "uk government and devolution." The dataset includes petition text, entity information (`has_entity`), and other metadata. The model leverages text preprocessing, feature engineering, and hyperparameter tuning to achieve robust performance.

### Key Features
- **Data Preprocessing**: Text cleaning, tokenization, stopword removal, and lemmatization using NLTK.
- **Feature Engineering**: TF-IDF vectorization for text and label encoding for entity data.
- **Model**: Linear Support Vector Classifier (LinearSVC) with GridSearchCV for hyperparameter tuning.
- **Evaluation**: Achieves a test accuracy of 91% and meets specific performance criteria (e.g., <9% error rate for "uk government and devolution").

## Dataset
The dataset (`comp1804_coursework_dataset_24-25.csv`) is downloaded from Google Drive using `gdown`. It contains 8,898 rows with columns like `petition_text`, `has_entity`, `petition_topic`, and more. The project focuses on cleaning and processing `petition_text` and `has_entity` for classification.

## Requirements
To run this project, install the required Python packages:
```bash
pip install gdown pandas numpy scikit-learn nltk
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m "Add feature"`).
4. Push to your branch (`git push origin feature-branch`).
5. Open a Pull Request.

# Petition Topic Classifier
[![Python](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)

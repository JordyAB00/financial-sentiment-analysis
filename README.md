# Financial Sentiment Analysis

## Overview
This project analyzes sentiment in financial texts using Natural Language Processing (NLP) and Machine Learning techniques. The implementation includes text preprocessing, exploratory data analysis, and the evaluation of multiple classification models.

## Dataset
The dataset combines data from FiQA and Financial PhraseBank, providing financial sentences with sentiment labels (positive, negative, neutral). It contains over 5,800 labeled financial statements with an unbalanced class distribution.

## Methodology
1. **Data Exploration**: Analysis of class distribution, text length patterns, and word frequencies
2. **Text Preprocessing**: Tokenization, stopword removal, lemmatization
3. **Feature Engineering**: TF-IDF vectorization
4. **Model Implementation**: 
   - Multinomial Naive Bayes
   - Logistic Regression
   - Random Forest
5. **Model Evaluation**: Comparison based on accuracy, precision, recall, and F1-score

## Key Findings
- Strong class imbalance (53.7% neutral, 31.8% positive, 14.5% negative)
- Logistic Regression achieved the best performance with 69.29% accuracy
- All models struggled with detecting negative sentiment
- Key predictive terms include directional indicators ("long", "lower", "increased") and corporate activity terms ("signed", "buy", "acquisition")

## Interactive Notebook
The analysis is presented in an interactive Jupyter notebook that walks through the entire process from data exploration to model evaluation.

## Technologies Used
- Python (NLTK, scikit-learn, pandas)
- Jupyter Notebooks
- Data Visualization (matplotlib, seaborn)

## Future Improvements
- Address class imbalance with techniques like SMOTE
- Implement n-gram features to capture contextual patterns
- Explore advanced models like BERT or FinBERT
- Develop an API for real-time sentiment analysis

## Citation
Malo, Pekka, et al. "Good debt or bad debt: Detecting semantic orientations in economic texts." Journal of the Association for Information Science and Technology 65.4 (2014): 782-796.
# Sentiment Analysis Project

## Overview

This project evaluates the performance of different approaches to sentiment analysis. Three distinct techniques were employed, each with its unique methodology and accuracy results on the test dataset.

### Heuristic Approach using TextBlob

- **Methodology:** Assigns polarity scores to words using TextBlob.
- **Accuracy on Test Dataset:** 42%
- **Summary:** The TextBlob approach showcases effectiveness in preprocessing, text parsing, feature extraction, and sentiment polarity analysis. Its comprehensive functionalities contribute to a robust performance, achieving an accuracy of 42%.

### Finetuned Transformer Model (BERT)

- **Methodology:** Utilizes BERT Fine-Tuned Transformer for context understanding.
- **Accuracy on Test Dataset:** 44% using Multinomial Naïve Bayes ML Model.
- **Summary:** BERT excels due to pre-training on extensive corpora, transfer learning, and fine-tuning for specific tasks. Despite a modest accuracy of 44%, this can be attributed to the use of a very small dataset for training (approximately 2% of the entire processed dataset) due to significant computational requirements.

### Train Machine Learning Model with TF-IDF

- **Methodology:** Trains a Multinomial Naive Bayes ML model based on TF-IDF.
- **Accuracy on Test Dataset:** Approximately 63% with hyperparameter alpha = 0.1.
- **Summary:** Multinomial Naive Bayes applied to TF-IDF demonstrates high efficiency, suitability for multiclass classification, and effectiveness with text data. TF-IDF provides a meaningful representation of terms within documents, contributing to the model's accuracy.

### Train Machine Learning Model with Word Embedding

- **Methodology:** Trains a Logistic Regression ML model based on Word Embedding.
- **Accuracy on Test Dataset:** 45% with hyperparameters like vector_size and window.
- **Summary:** Despite inherent strengths in capturing semantic information, interpretability, and scalability, Logistic Regression on Word Embeddings exhibits suboptimal performance with an accuracy of 45%.

## Conclusion

This project highlights the strengths and limitations of various sentiment analysis techniques, providing insights into their applicability and effectiveness in different scenarios.

## FutureWork

The existing dataset exhibits a significant imbalance, with a scarcity of lower-rated data in comparison to higher ratings. This imbalance poses substantial challenges, particularly during testing in both Deep Learning and Machine Learning contexts. Additionally, fine-tuning a transformer model demands considerable computational power, necessitating the use of supercomputers or GPU systems. To illustrate, my laptop encountered operational interruptions on multiple occasions while attempting to apply BERT on just 12% of the dataset.
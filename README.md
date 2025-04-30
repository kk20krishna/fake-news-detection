# Fake News Detection Using Semantic Classification

This project addresses the widespread issue of **fake news** by developing a machine learning system that classifies news articles as either **true** or **fake** using **Word2Vec embeddings** and supervised learning models. It was created as part of an academic assignment by **Krishna Kumar S.** and **Varun B.**

---

## Table of Contents

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [Dataset Overview](#dataset-overview)
4. [Preprocessing](#preprocessing)
5. [Methodology](#methodology)
6. [Techniques Used](#techniques-used)
7. [Key Insights](#key-insights)
8. [Results](#results)
9. [Conclusion](#conclusion)
10. [Assumptions](#assumptions)

---

## Introduction

Fake news spreads rapidly in the digital age, undermining public trust. This project applies **semantic classification** using **Word2Vec** to detect fake news articles. The goal is to build a supervised model that improves information reliability online.

---

## Problem Statement

Develop a system that:
- Automatically classifies news articles as real or fake.
- Uses semantic features (not just syntactic) to improve robustness and accuracy.

---

## Dataset Overview

- Two datasets: `True.csv` (21,417 articles) and `Fake.csv` (23,502 articles).
- Each entry includes:
  - `title`: Headline of the news article
  - `text`: Main content
  - `label`: 1 = Real, 0 = Fake

---

## Preprocessing

1. **Cleaning**: Lowercasing, removing punctuation, square brackets, and numeric words.
2. **Tokenization**: Splitting into words.
3. **POS Tagging**: Grammatical tagging (e.g., noun, verb).
4. **Lemmatization**: Converting words to their root form.
5. **Stop Word Removal**: Common word filtering; retained only `NN` and `NNS`.

---

## Methodology

- **Data Preparation**: Merged datasets and cleaned text.
- **Train/Validation Split**: Stratified sampling.
- **EDA**: Word clouds, character analysis, and n-gram frequencies.
- **Feature Extraction**: Applied **Word2Vec** for semantic representation.
- **Model Training**: Evaluated Logistic Regression, Decision Tree, and Random Forest.

---

## Techniques Used

- **Word2Vec** for semantic vectorization
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- Evaluation Metrics: **Accuracy, Precision, Recall, F1-Score**

---

## Key Insights

- **True News**:
  - Used neutral language.
  - Referenced official sources (e.g., "said", "state", "official").
- **Fake News**:
  - Sensational and emotional language.
  - Frequent mention of individuals like "Trump", "Clinton", "Hillary".

- **Model Performance**:
  - **Logistic Regression**: Accuracy 94%, F1 0.94
  - **Decision Tree**: Accuracy 84%, F1 0.83
  - **Random Forest**: Accuracy 93%, F1 0.92 (Best balance between precision and recall)

---

## Results

- **Logistic Regression Forest** outperformed other models on both accuracy and F1-score.
- **F1-score** was chosen as the primary metric to balance false positives and false negatives.

---

## Conclusion

The semantic classification approach using Word2Vec was successful in differentiating between true and fake news. This method, especially with **Logisric regressiona and Random Forest**, showed strong potential to minimize misinformation online.

---

## Assumptions

- The pre-trained **Word2Vec** model captures semantic meaning well.
- The dataset is representative of typical news content.

---

## Authors

- **Krishna Kumar S.**
- **Varun B.**

---

## License

This project is intended for educational purposes only.


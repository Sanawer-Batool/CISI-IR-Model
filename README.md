# CISI-IR-Model
This repository contains a Jupyter Notebook implementation of three information retrieval (IR) models—TF-IDF with Cosine Similarity, SMART Notation TF-IDF (ltc.lnc), and BM25—applied to the CISI dataset.

# CISI Dataset Information Retrieval Models

## Overview
This repository contains a Jupyter Notebook implementation of three information retrieval (IR) models applied to the CISI dataset. The project demonstrates preprocessing, model training, evaluation, and visualization of results, serving as a practical example for IR techniques.

## Project Description
The CISI dataset, consisting of document abstracts (`CISI.ALL`), queries (`CISI.QRY`), and relevance judgments (`CISI.REL`), is used to evaluate the following models:
- **Model A (TF-IDF)**: Uses TF-IDF with cosine similarity for document ranking.
- **Model B (SMART)**: Implements SMART notation TF-IDF with `ltc.lnc` weighting.
- **Model C (BM25)**: Employs the BM25 algorithm with tuned parameters (`k1=1.5`, `b=0.75`).

The workflow includes:
- **Preprocessing**: Lowercasing, tokenization, stop word removal, and Porter stemming.
- **Evaluation**: Calculation of average precision and recall based on `CISI.REL`.
- **Visualization**: A bar chart comparing model performance using matplotlib.

## Results
- **Model A (TF-IDF)**: Precision = 0.3526, Recall = 0.1314
- **Model B (SMART)**: Precision = 0.3658, Recall = 0.1433
- **Model C (BM25)**: Precision = 0.3684, Recall = 0.1531
BM25 (Model C) outperformed the other models, showing the highest precision and recall.

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required libraries:
  - `nltk` (for preprocessing)
  - `scikit-learn` (for TF-IDF and cosine similarity)
  - `rank_bm25` (for BM25)
  - `matplotlib` (for visualization)
  - `numpy` (for numerical operations)

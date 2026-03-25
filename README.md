# IMDB Sentiment Classifier (NLP Course Project)

A complete NLP assignment project for sentiment classification on the IMDB 50K movie reviews dataset.

This repository combines:
- Classical NLP pipelines (BoW and TF-IDF)
- Multiple machine learning classifiers (Naive Bayes, Logistic Regression, Linear SVM, SGD)
- Deep learning baselines (RNN, LSTM, small Transformer)
- Unified model comparison with metrics and plots

## Why this project

This project was built to demonstrate core topics from an NLP course in one end-to-end workflow:
- data collection and cleaning
- feature engineering
- model training and evaluation
- hyperparameter tuning
- error analysis and interpretation

## Dataset

- Source: IMDB Dataset of 50K Movie Reviews
- Downloaded with `kagglehub`
- Kaggle dataset id: `lakshmi25npathi/imdb-dataset-of-50k-movie-reviews`

## Main notebook

- [imdb_nlp_classification.ipynb](imdb_nlp_classification.ipynb)

The notebook includes:
1. environment setup and imports
2. dataset download with KaggleHub
3. exploratory data analysis
4. preprocessing pipeline (light and aggressive variants)
5. classical model baselines
6. hyperparameter tuning with cross-validation
7. deep learning models (RNN, LSTM, Transformer)
8. final comparison across all models

## Tech stack

- Python
- pandas, numpy
- scikit-learn
- nltk
- PyTorch
- matplotlib, seaborn
- uv for dependency management

## Quickstart

### 1) Clone

```bash
git clone <your-repo-url>
cd Movie-classificator
```

### 2) Install dependencies

```bash
uv sync
```

### 3) Run notebook

Open [imdb_nlp_classification.ipynb](imdb_nlp_classification.ipynb) and run cells top to bottom.

## Project structure

```text
.
|-- imdb_nlp_classification.ipynb
|-- pyproject.toml
|-- uv.lock
|-- LICENSE
`-- README.md
```

## Evaluation metrics

Models are compared with:
- Accuracy
- Precision
- Recall
- F1 score
- ROC-AUC (when available)

The notebook ends with a final leaderboard-style comparison plot so you can discuss results clearly in a report or presentation.

## Notes on results

Classical TF-IDF + linear models are very strong on this dataset and often outperform smaller deep models unless deep models are carefully tuned.

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file.

---

If you are a recruiter, instructor, or teammate reviewing this repository: the notebook is designed to be presentation-friendly and reproducible with a single `uv sync`.
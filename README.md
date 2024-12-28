
### README

This repository provides a solution for multi-label text classification to detect toxic comments using machine learning. The task is to classify comments into multiple categories such as "toxic", "severe_toxic", "obscene", etc.

### Features

- **Text Preprocessing**: Removes stopwords, cleans, and stems text data.
- **Multi-Label Classification**: Uses Logistic Regression and Naive Bayes classifiers.
- **Model Evaluation**: Evaluates models using ROC-AUC and accuracy.
- **ROC Curve**: Plots ROC curves for model performance.

### Setup

Install dependencies using:
```bash
pip install -r requirements.txt
```

### Workflow

1. Load the dataset (`train.csv`).
2. Preprocess text data (remove stopwords, clean, and stem).
3. Train models using a pipeline with TfidfVectorizer and OneVsRestClassifier.
4. Evaluate models and plot ROC curves.

### Example Usage

```python
sentence = 'hello dick wikipedia fuckwhit ban'
results = LR_pipeline.predict([sentence])
```


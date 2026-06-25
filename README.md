# U.S. Presidential Inaugural Address Analysis
### Digital Humanities 101 – Final Individual Coding Project
**Author:** Joey Wong

---

## Project Overview

This project investigates the following research question:

> **How has the language of U.S. presidential inaugural addresses changed over time, and what can computational methods reveal about shifting political priorities and national moods?**

To explore this question, I analyze more than two centuries of U.S. presidential inaugural addresses using several computational text analysis methods introduced throughout Digital Humanities 101, including:

- Word Frequency Analysis
- Historical Comparison of Key Political Terms
- Sentiment Analysis
- Exploratory Topic Modeling (additional analysis beyond the course requirements)

The project uses Python and Jupyter Notebook to preprocess text, analyze rhetorical patterns, visualize results, and interpret findings within their historical context.

---

# Dataset

This project uses the **NLTK Inaugural Address Corpus**.

Unlike downloading individual speeches from Project Gutenberg, the corpus is distributed directly through the Natural Language Toolkit (NLTK) and can be accessed programmatically.

The corpus contains inaugural addresses from:

- George Washington (1789)
- ...
- Donald Trump (2025)

No external data download is required beyond installing the NLTK corpus.

---

# Repository Contents

```
.
├── DH101_Joey_Final_Proj.ipynb
├── inaugural_addresses.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

# Requirements

This project was developed using

- Python 3.9+
- Jupyter Notebook
- VS Code

Required Python packages include:

- pandas
- matplotlib
- nltk
- scikit-learn

---

# Setting Up the Project

## 1. Clone the repository

```bash
git clone <repository-url>
cd <repository-folder>
```

---

## 2. Create a virtual environment

### macOS / Linux

```bash
python3 -m venv .venv
```

### Windows

```bash
python -m venv .venv
```

---

## 3. Activate the virtual environment

### macOS / Linux

```bash
source .venv/bin/activate
```

### Windows

```cmd
.venv\Scripts\activate
```

Once activated, your terminal should display something similar to

```
(.venv)
```

---

## 4. Install the required packages

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install pandas matplotlib nltk scikit-learn
```

---

## 5. Download the NLTK datasets

The notebook downloads the required corpora automatically. Run through all the cells.

Alternatively, run:

```python
import nltk

nltk.download("inaugural")
nltk.download("punkt_tab")
nltk.download("stopwords")
nltk.download("vader_lexicon")
```

These resources are only downloaded once.

---

## 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

or

```bash
jupyter lab
```

Open

```
DH101_Joey_Final_Proj.ipynb
```

and run the notebook from top to bottom.

---

# Project Workflow

The notebook follows this workflow:

1. Import libraries
2. Download the NLTK Inaugural Address Corpus
3. Access and inspect the dataset
4. Build a pandas DataFrame
5. Clean and standardize the text
6. Tokenize speeches and remove stopwords
7. Perform word frequency analysis
8. Visualize the most common words
9. Compare key political terms across historical periods
10. Perform sentiment analysis
11. Compare sentiment across historical periods
12. Conduct an exploratory topic modeling analysis

---

# Methods Used

### Word Frequency Analysis

Measures how often words appear across all inaugural addresses to identify recurring rhetorical themes.

### Historical Comparison

Compares the frequency of selected political terms (e.g., *freedom*, *union*, *democracy*, *security*, and *economy*) across different historical periods.

### Sentiment Analysis

Uses NLTK's VADER Sentiment Analyzer to estimate the emotional tone of each inaugural address.

### Topic Modeling (Exploratory)

As an extension beyond the original project proposal, I implemented Latent Dirichlet Allocation (LDA) using Scikit-Learn to explore broader thematic patterns across the corpus.

---

# Notes

The topic modeling section was completed independently after receiving feedback on my proposal. It is intended as an exploratory extension rather than one of the primary analytical methods required by the course.

In addition, debugging was made with the help of Claude Code. 

---

# License

This project was completed as part of Digital Humanities 101 at UC Berkeley for educational purposes.

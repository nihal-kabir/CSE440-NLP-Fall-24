# CSE440 Natural Language Processing – Assignments

## Overview

This repository contains my completed coursework for **CSE440 – Natural Language Processing** at BRAC University. It currently hosts two fully‑executed Jupyter notebooks that walk through classic and modern NLP pipelines, from corpus statistics to deep‑learning sequence models.

* **Assignment 1 – Text Analysis, Processing & Representation**: exploratory analysis of *Moby‑Dick*, IMDB review cleaning, TF‑IDF vectorisation, and word‑embedding arithmetic.
* **Assignment 2 – Sequence Learning**: sentiment‑classification models on IMDB reviews using bag‑of‑words, TF‑IDF, and a shallow recurrent neural network.


---

## Repository layout

```text
.
├── 440_assignment_1.ipynb   # Notebook for Assignment 1
├── 440_assignment_2.ipynb   # Notebook for Assignment 2
├── CSE440 A‑1.pdf       # Spec for Assignment 1
│── CSE440 A‑2.pdf       # Spec for Assignment 2
└── README.md                # You are here
```

---

## Quick start

1. **Clone the repo**

   ```bash
   git clone https://github.com/nihal-kabir/CSE440‑NLP‑Fall-24.git
   cd CSE440‑NLP‑Fall-24
   ```
2. **Create a virtual environment** *(optional but recommended)*

   ```bash
   python -m venv .venv
   source .venv/bin/activate   # Windows: .venv\Scripts\activate
   ```
3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```
4. **Launch the notebooks**

   ```bash
   jupyter lab
   # OR
   # jupyter notebook
   ```


## Environment

The notebooks were developed with the stack below; newer versions should work, but these are known‑good:

| Tool               | Version |
| ------------------ | ------- |
| Python             | 3.10    |
| JupyterLab         | 4.x     |
| pandas             | 2.x     |
| nltk               | 3.x     |
| scikit‑learn       | 1.5     |
| PyTorch            | 2.3     |
| TensorFlow / Keras | 2.19    |

Install with `pip install -r requirements.txt` or recreate the conda environment via `environment.yml` if provided.

---

## Datasets

| Dataset                    | Size   | Source                                                                               | Used in |
| -------------------------- | ------ | ------------------------------------------------------------------------------------ | ------- |
| IMDB Movie Reviews         | 50 K   | Course Google Drive link (see notebook)                                              | A1, A2  |
| GloVe 6B, 100‑d embeddings | 822 MB | [https://nlp.stanford.edu/projects/glove/](https://nlp.stanford.edu/projects/glove/) | A1      |
| `nltk.book` corpora        | –      | Via NLTK downloader (`nltk.downloader popular`)                                      | A1      |

> **Note**: Large datasets are excluded from version control. The notebooks include helper code to fetch and cache them automatically.

---

## Assignment summaries

### Assignment 1 – Text Analysis

* Corpus statistics for *Moby‑Dick* (vocabulary size, word counts, frequency ranks)
* IMDB review preprocessing – stop‑word removal, punctuation stripping, lower‑casing
* TF‑IDF feature extraction and inspection
* Word‑embedding arithmetic with pre‑trained GloVe vectors (e.g., `king − man + woman ≈ queen`)

### Assignment 2 – Sequence Learning

* Bag‑of‑words vs. TF‑IDF baselines (Logistic Regression & Multinomial Naive Bayes)
* Shallow RNN with pre‑trained embeddings (Keras Sequential model)
* Performance comparison and visualisation

---

## Reproducing the results

The notebooks set `random_state` where applicable for deterministic runs. GPU acceleration (CUDA) is detected automatically but is *not* required.

---

## Contributing

Pull requests that fix issues, improve clarity, or extend experiments are welcome! Please open an issue first to discuss substantial changes.



---

## Acknowledgements

* **Dr. Farig Yousuf Sadeque** – course instructor and assignment author
* Open‑source communities behind NLTK, scikit‑learn, PyTorch, and Keras

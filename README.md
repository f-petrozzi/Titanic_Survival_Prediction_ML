# Titanic Survival Prediction Model
A short, end‑to‑end classification project that predicts passenger survival on the RMS Titanic using two straightforward algorithms.

[![Watch on YouTube](https://img.shields.io/badge/Walkthrough-Video-red?logo=youtube)](https://www.youtube.com/watch?v=IucFNaEQSFM)

## Motivation
The Titanic dataset is a classic starter problem for classification.  It is small, well‑labeled, and highlights common data‑science steps: cleaning, feature engineering, model comparison, and simple interpretability.

## Dataset
* **Source:** [Kaggle – Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)
* **Rows:** 891 training passengers  |  418 test passengers  
* **Key features:** `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`, plus engineered fields  
* **Target:** `Survived` (0 = No, 1 = Yes)

## Models
| Model | Why chosen | Key metric* |
|-------|------------|-------------|
| Gaussian Naïve Bayes | Fast baseline for tabular data | `accuracy = 78%`, `F1 (weighted) = 78%` |
| Decision Tree | Simple, interpretable tree of rules | `accuracy = 80%`, `F1 (weighted) = 80%` |


## Quick Walk‑through
Click the badge above or watch the [YouTube video](https://www.youtube.com/watch?v=IucFNaEQSFM) for a 7‑minute code tour.

---

## Getting Started

```bash
# clone
git clone https://github.com/f-petrozzi/titanic_survival_prediction.git
cd titanic_survival_prediction

# create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# install requirements
pip install -r requirements.txt

# launch Jupyter
jupyter notebook
```

## Requirements
Python 3.9+ and the packages in `requirements.txt`
(mainly `pandas`, `numpy`, `scikit‑learn`, `jupyter`).

## Download the data
```bash
pip install kaggle
kaggle competitions download -c titanic -p data/
unzip data/titanic.zip -d data/
```

## Reflection
* Small, tidy datasets are ideal for learning the full ML cycle.  
* A plain Decision Tree can match or beat Naïve Bayes once hyper‑parameters are tuned.
* Feature scaling mattered little here; handling missing ages mattered a lot.

---

## License
MIT © 2025 Fabrizio Petrozzi

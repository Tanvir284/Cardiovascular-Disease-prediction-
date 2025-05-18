# Cardiovascular Disease Prediction

This repository contains sample notebooks for predicting cardiovascular disease using the [Kaggle cardiovascular disease dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset).

## Dataset origin

The data comes from Kaggle and consists of medical examination records with a target indicating whether a patient has cardiovascular disease. A copy of `cardio_train.csv` is provided for convenience. See the Kaggle page for the full description and license terms.

## Prerequisites

- Python 3.10 or later
- Recommended packages: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `lightgbm`, and `jupyter` for running the notebooks.

Install the requirements with:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost lightgbm jupyter
```

## Running the notebooks

1. Start Jupyter:
   ```bash
   jupyter notebook
   ```
2. Open either `cardiovascular-disease.ipynb` or `cardio-disease-modeling-73-79-accuracy.ipynb` and execute the cells in order. The notebooks load `cardio_train.csv`, perform preprocessing and training, and then evaluate the models.

Alternatively you can convert a notebook to a script and run it from the command line:

```bash
jupyter nbconvert --to script cardiovascular-disease.ipynb
python cardiovascular-disease.py
```

## Expected results

Accuracy varies between models. Logistic Regression achieves about 72% accuracy with a cross-validation mean near 71%. Tree-based models such as XGBClassifier, LGBMClassifier, and a stacking ensemble reach roughly **73–74%** accuracy on the provided test split. Results are reported using `accuracy_score`, `classification_report`, and cross‑validation scores.

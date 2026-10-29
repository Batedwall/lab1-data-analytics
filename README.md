# Lab 1: Introduction to Data Analytics and Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Batedwall/lab1-data-analytics/blob/main/notebooks/Zavdannia1_Pasovystiy.ipynb)

- **Author:** Yulian Pasovystiy
- **Group:** CS-41
- **Course:** Data Analytics

## Description

This repository contains the first practical assignment on data analytics.
The goal is to learn how to create notebooks in the cloud environment
Google Colab, load and inspect tabular data with **Pandas**, and perform
basic vectorized computations with **NumPy**.

## Dataset

Coffee shop sales data, stored in the `data/` folder:

| File | Rows | Columns | Period |
|------|------|---------|--------|
| `index_1.csv` | 3636 | `date`, `datetime`, `cash_type`, `card`, `money`, `coffee_name` | 2024-03-01 – 2025-03-23 |
| `index_2.csv` | 262 | `date`, `datetime`, `cash_type`, `money`, `coffee_name` | 2025-02-08 – 2025-03-23 |

Each row is a single transaction. `money` is the payment amount,
`cash_type` is the payment method (card or cash), and `coffee_name` is the
name of the drink. In `index_1.csv`, the `card` column is empty for some
transactions.

## Project structure

```
lab1-data-analytics/
├── README.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   └── Zavdannia1_Pasovystiy.ipynb   # Tasks 1–7 and the bonus task
└── data/
    ├── index_1.csv
    └── index_2.csv
```

## Contents of the notebook

1. Importing `pandas` and `numpy`, printing their versions
2. Reading a CSV file into a DataFrame, `head(3)` and `tail(3)`
3. Inspecting `df.columns` and its type
4. One-dimensional NumPy array: sum, mean, min, max, multiplication
5. 3×3 random integer array, aggregation with `axis=0` and `axis=1`
6. Markdown cell: heading, list, bold text, benefits of text cells
7. Mounting Google Drive, reading a CSV, `df.info()`, comparing data types
8. ★ Bonus: combined analysis (`head`, `shape`, `info`, `describe`, NumPy mean of the `money` column)

## How to run

1. Click the **Open in Colab** badge above (or upload the notebook to
   [Google Colab](https://colab.research.google.com) manually).
2. Upload `index_1.csv` and `index_2.csv` to the root of your Google Drive
   (`My Drive`).
3. Run the cells from top to bottom (`Shift + Enter`).
   Grant access to Google Drive when prompted.

To run locally instead, install the dependencies and open the notebook in
Jupyter (remove the `google.colab` cells and change file paths to `data/...`):

```bash
pip install -r requirements.txt
jupyter notebook
```

## Technologies

- Python 3
- Google Colab
- pandas
- NumPy

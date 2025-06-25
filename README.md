# 🚢 Titanic ETL Pipeline - Internship Task 1

This project demonstrates an **ETL (Extract, Transform, Load)** data pipeline using a sample **Titanic dataset**. It was created as part of the Data Science Internship program to show how data preprocessing works using Python and Scikit-learn.

---

## 📌 Objective

The goal is to:
- Simulate real-world data handling using a subset of the Titanic dataset.
- Build an automated preprocessing pipeline.
- Save the transformed data and pipeline for future use.

---

## 📁 Files Included

| File Name                     | Description                                  |
|------------------------------|----------------------------------------------|
| `titanic_etl_pipeline.ipynb` | Jupyter Notebook with full ETL process       |
| `titanic_sample.csv`         | Sample dataset used in the notebook          |
| `X_train.npy`, `X_test.npy`  | Processed feature data (NumPy arrays)        |
| `y_train.csv`, `y_test.csv`  | Target data for training/testing             |
| `etl_pipeline.joblib`        | Saved Scikit-learn pipeline                  |
| `README.md`                  | Project documentation                        |

---

## ⚙️ Tools & Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Joblib (for saving pipeline)
- Jupyter Notebook

---

## 🔄 Pipeline Process

### ✅ 1. Extract
- Load a mini version of Titanic dataset from `titanic_sample.csv`.
- Explore structure and identify missing values.

### 🔧 2. Transform
- Create preprocessing pipelines for:
  - Numeric columns: Mean imputation + StandardScaler
  - Categorical columns: Most frequent imputation + OneHotEncoder
- Use `ColumnTransformer` to combine both.
- Split the data using `train_test_split`.

### 💾 3. Load
- Save the transformed training and testing data (`.npy`, `.csv`).
- Save the complete preprocessing pipeline using `joblib`.

---

## 🚀 How to Run

1. Clone this repository or download the files.

2. Install dependencies:

```bash
pip install pandas numpy scikit-learn joblib

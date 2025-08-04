# Titanic Dataset: Data Cleaning and Preprocessing

This repository contains the complete data cleaning and preprocessing steps applied to the Titanic dataset. The goal is to prepare the data for machine learning models by handling missing values, encoding categorical variables, scaling numerical features, and removing outliers.

---

## 📁 Files Included

- `task1.ipynb` – Jupyter Notebook with full preprocessing code
- `cleaned_titanic.csv` – Final cleaned dataset after preprocessing
- `Titanic_Dataset.csv` – original dataset
- `README.md` – This documentation file

---

## 📊 Dataset Overview

The original Titanic dataset contains information about passengers, including:
- Demographics (Age, Sex)
- Ticket and fare details
- Class and cabin
- Survival status

---

## 🔧 Preprocessing Steps

1. **Import and Explore Data**
   - Loaded the dataset using `pandas`
   - Explored structure, column types, and null values

2. **Handle Missing Values**
   - `Age`: Filled with **median**
   - `Embarked`: Filled with **mode**
   - `Cabin`: Dropped due to too many missing entries

3. **Convert Categorical Features**
   - `Sex`: Converted using **Label Encoding**
   - `Embarked`: Converted using **One-Hot Encoding**

4. **Standardize Numerical Features**
   - Used `StandardScaler` to scale `Age` and `Fare`

5. **Outlier Detection and Removal**
   - Used **boxplot** for visual inspection
   - Removed outliers in `Fare` using **IQR method**

---

## 🧠 Tools & Libraries Used

- Python
- Pandas
- NumPy
- Seaborn & Matplotlib
- Scikit-learn

---

## ✅ Output

The cleaned dataset is saved as `cleaned_titanic.csv` and is ready for use in machine learning models or further analysis.

---

## 📌 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/rakshitha-kolla/task1_dataCleaning_preprocessing.git

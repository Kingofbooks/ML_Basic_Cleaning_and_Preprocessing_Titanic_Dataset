# ML_Basic_Cleaning_and_Preprocessing_Titanic_Dataset

# Titanic Data Preprocessing and Exploration 🛳️

This project focuses on **cleaning, preprocessing, and visualizing** the Titanic dataset from Kaggle to prepare it for machine learning models.

## 📁 Dataset
The dataset used is `Titanic-Dataset.csv`, containing details about passengers on the Titanic like age, gender, class, and survival.

---

## 🧠 Steps Performed

### 1. Import & Explore
- Loaded the dataset using pandas
- Checked for null values and data types
- Displayed basic stats and column info

### 2. Handle Missing Values
- Filled missing `Age` with the median
- Filled missing `Embarked` with the most common value (S)

### 3. Encode Categorical Features
- Converted `Sex`: male → 0, female → 1
- Converted `Embarked` using one-hot encoding (`Embarked_Q`, `Embarked_S`)

### 4. Normalize / Standardize Features
- Applied `StandardScaler` to `Age` and `Fare` to bring them to a similar scale

### 5. Detect and Remove Outliers
- Used boxplots to visualize outliers
- Removed outliers from numerical features (`Age`, `Fare`, `SibSp`, `Parch`) using IQR method
- Plotted before-and-after boxplots to see the changes

---

## 📊 Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

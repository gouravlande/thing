# Insurance Dataset - Exploratory Data Analysis (EDA)

## Project Overview

This project performs Exploratory Data Analysis (EDA) on an Insurance Dataset using Python libraries such as:

- NumPy
- Pandas
- Matplotlib
- Seaborn

The main goal of this notebook is to:
- Understand dataset structure
- Analyze features
- Detect patterns
- Check missing values
- Visualize distributions
- Prepare data for Machine Learning

---

# Dataset Information

The dataset contains insurance-related information with the following features:

| Column | Description |
|---|---|
| age | Age of the person |
| sex | Gender |
| bmi | Body Mass Index |
| children | Number of children |
| smoker | Smoking status |
| region | Residential region |
| charges | Medical insurance charges |

---

# Libraries Used

```python
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
```

---

# Steps Performed in EDA

## 1. Importing Libraries

Required libraries for:
- Numerical operations
- Data analysis
- Data visualization

---

## 2. Loading Dataset

```python
df = pd.read_csv('/content/insurance (1).csv')
```

The dataset is loaded into a Pandas DataFrame.

---

## 3. Understanding Dataset

### Viewing Dataset

```python
df
```

Displays complete dataset.

---

### Shape of Dataset

```python
df.shape
```

Output:

```python
(1338, 7)
```

Meaning:
- 1338 rows
- 7 columns

---

### Dataset Information

```python
df.info()
```

Used to check:
- Data types
- Null values
- Memory usage

---

### Statistical Summary

```python
df.describe()
```

Provides:
- Mean
- Standard deviation
- Minimum value
- Maximum value
- Quartiles

---

# Missing Value Analysis

```python
df.isnull().sum()
```

Purpose:
- Detect missing values in dataset

Result:
- No missing values found.

---

# Feature Analysis

## Numerical Columns

```python
numeric_columns = ['age', 'bmi', 'children', 'charges']
```

These columns are analyzed using histograms.

---

# Data Visualization

## Histogram Plot

```python
for col in numeric_columns:
    plt.figure(figsize=(6,4))
    sns.histplot(df[col], kde=True, bins=20)
```

Purpose:
- Understand data distribution
- Detect skewness
- Identify outliers

---

# EDA Concepts Covered

- Data understanding
- Descriptive statistics
- Distribution analysis
- Null value detection
- Data visualization
- Feature analysis

---

# Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Visualization |
| Seaborn | Statistical Visualization |
| Google Colab | Development Environment |

---

# Project Workflow

```text
Import Libraries
       ↓
Load Dataset
       ↓
Understand Dataset
       ↓
Check Missing Values
       ↓
Statistical Summary
       ↓
Visualization
       ↓
Feature Analysis
```

---

# Learning Outcomes

After completing this project, I learned:

- How to perform EDA
- Understanding dataset structure
- Data visualization techniques
- Statistical analysis
- Identifying patterns in data
- Preparing data for preprocessing and Machine Learning

---

# Future Improvements

- Outlier Detection
- Feature Engineering
- Encoding
- Feature Scaling
- Correlation Heatmap
- Machine Learning Model Building

---

# Author

## Gourav Lande

Aspiring:
- AI Engineer
- Machine Learning Engineer
- Data Scientist

GitHub:
https://github.com/gouravlande

---

# Repository Link

https://github.com/gouravlande/thing.git

---

# Conclusion

This project demonstrates the fundamental process of Exploratory Data Analysis (EDA) using Python and visualization libraries. EDA is an essential step before applying Machine Learning algorithms because it helps understand the dataset and improve data quality.

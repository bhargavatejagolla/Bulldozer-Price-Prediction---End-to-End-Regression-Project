# 🚜 Bulldozer Price Prediction - End-to-End Regression Project

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-brightgreen)
![Regression](https://img.shields.io/badge/Regression-Analysis-yellow)

## 📋 Project Overview

This project implements an end-to-end machine learning solution to predict the sale price of bulldozers using historical auction data. The goal is to build a regression model that minimizes the Root Mean Squared Log Error (RMSLE) between predicted and actual auction prices.

**Competition Source:** [Kaggle Bluebook for Bulldozers](https://www.knnuggets.com/2021/05/bluebook-bulldozer-price-prediction.html)

## 🎯 Problem Statement

> How well can we predict the future sale price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?

## 📊 Dataset

The dataset consists of three main files from the Kaggle competition:
- **Train.csv** - Training set with data through the end of 2011
- **Valid.csv** - Validation set with data from January 1, 2012 - April 30, 2012
- **Test.csv** - Test set with data from May 1, 2012 - November 2012

### Dataset Characteristics
- **Size:** 412,698 entries with 53 features
- **Feature Types:** Mixed (numerical, categorical, datetime)
- **Key Columns:** SalesID, SalePrice, MachineID, ModelID, YearMade, saledate, and various bulldozer specifications

## 📈 Evaluation Metric

The competition uses **Root Mean Squared Log Error (RMSLE)** as the evaluation metric:

$$
\text{RMSLE} = \sqrt{\frac{1}{n}\sum_{i=1}^{n}\Big(\log(p_i + 1) - \log(a_i + 1)\Big)^2}
$$

Where:  
- $p_i$ is the predicted price  
- $a_i$ is the actual price  
- $n$ is the total number of observations  


## 🛠️ Technical Implementation

### Libraries Used
```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import sklearn
# Bulldozer Price Prediction
```
## 📊 Current Progress
- ✅ Data loading and initial exploration  
- ✅ Basic data analysis and visualization  
- ✅ Date parsing for time series analysis  
- 🔄 Data preprocessing and cleaning  
- 🔄 Feature engineering  
- 🔄 Model building and evaluation  

---

## 🔑 Key Analysis Steps

### Data Loading & Exploration
- Loaded training dataset with **412,698 entries** and **53 features**  
- Identified mixed data types (numerical and categorical)  
- Analyzed missing values across all columns  

### Initial Visualization
- Scatter plot of sale date vs. sale price  
- Histogram of sale price distribution  
- Temporal analysis of auction patterns  

### Data Preprocessing
- Parsed datetime format for `saledate` column  
- Initial handling of missing values  
- Basic statistical analysis  

---

## 🚀 Next Steps
- Comprehensive data cleaning and missing value imputation  
- Feature engineering and selection  
- Time-based feature creation from `saledate`  
- Categorical variable encoding  
- Model selection and hyperparameter tuning  
- Cross-validation and model evaluation  
- Submission preparation for Kaggle competition  

---

## 📁 Project Structure
```bash
bulldozer-price-prediction/
│
├── data/
│ ├── TrainAndValid.csv
│ ├── Test.csv
│ └── Valid.csv
│
├── notebooks/
│ └── end-to-end-bluebook-bulldozer-price-regression-video.ipynb
│
├── README.md
└── requirements.txt
```

---

## 👨‍💻 Author
**Bhargava Teja Golla**  

- GitHub: [bhargavatejagolla](https://github.com/bhargavatejagolla)  
- LinkedIn: [Golla Bhargava Teja](https://www.linkedin.com/in/golla-bhargava-teja/)  

---

## 📄 License
This project is for **educational purposes** as part of a machine learning portfolio.  
The dataset is provided by **Kaggle** for competition use.  

---

## 🤝 Contributing
This is a **personal project** for skill development.  
Suggestions and feedback are welcome through **issues or pull requests**.  

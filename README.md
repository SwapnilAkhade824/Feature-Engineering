# 🚗 Car Price Prediction — Feature Engineering and Data Preprocessing

### 👤 Submitted by: **Swapnil Santosh Akhade**  
**Department:** Artificial Intelligence and Machine Learning (A1)  
**Date:** 2 November 2025  

---

## 📘 Project Overview

This project focuses on performing **Feature Engineering** and **Data Preprocessing** on a publicly available **Car Price Prediction** dataset from Kaggle.  
The goal is to clean, transform, and prepare the dataset for machine learning applications, ensuring all features are numerical, consistent, and scaled for model training.

---

## 📂 Dataset Details

**Source:** [Kaggle - Car Price Prediction Dataset](https://www.kaggle.com/datasets/zafarali27/car-price-prediction)  
**Type:** Regression Problem  
**Target Variable:** `Price`

**Key Features:**
- Brand  
- Model  
- Engine Size  
- Fuel Type  
- Transmission  
- Mileage  
- Condition  
- Year  

---

## ⚙️ Steps Performed

### 1️⃣ Data Loading and Exploration
- Loaded dataset using pandas  
- Checked data types, missing values, and unique counts  

### 2️⃣ Handling Missing Values
- Numerical columns filled with **mean**
- Categorical columns filled with **mode**

### 3️⃣ Encoding Categorical Variables
- **Transmission** → Label Encoding  
- **Condition**, **Fuel Type**, **Brand** → One-Hot Encoding  
- **Model** → Label Encoding (to reduce feature explosion)

### 4️⃣ Feature Scaling
- Standardized numerical features using **StandardScaler**

### 5️⃣ Feature Selection
- Used **SelectKBest (f_regression)** to select top 10 important features  

### 6️⃣ Dimensionality Reduction
- Applied **PCA (Principal Component Analysis)** to reduce dimensionality  
- Visualized first two principal components with price as color gradient  
- Plotted explained variance ratio to analyze feature contribution  

---

## 📊 Outputs and Results
- Dataset transformed into fully numeric, standardized format  
- PCA visualization clearly shows data variance  
- Top 10 most important features identified via SelectKBest  
- Dataset ready for model training and regression tasks  

---

## ⚖️ Ethical Considerations
Although this dataset doesn’t include sensitive personal attributes, in real-world scenarios, including features like **Gender**, **Race**, or **Marital Status** can lead to biased predictions.  
To mitigate bias:
- Exclude sensitive features from the model  
- Regularly monitor fairness metrics  
- Maintain transparency in feature selection  

---

## 💻 Tools and Libraries Used
- **Python 3**
- **Google Colab**
- **Pandas**, **NumPy**
- **Scikit-learn**
- **Matplotlib**, **Seaborn**

---

## 🧾 How to Run
1. Open the `.ipynb` notebook in Google Colab or Jupyter Notebook  
2. Run all cells sequentially  
3. Ensure required libraries are installed (`!pip install kagglehub pandas numpy scikit-learn matplotlib seaborn`)  
4. The output visualizations and processed data will appear inline  

---

## 📌 Author
**Swapnil Santosh Akhade**  
B.Tech — Artificial Intelligence & Machine Learning  

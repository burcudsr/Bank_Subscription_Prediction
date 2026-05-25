# 🏦 Bank Marketing Prediction Model

This project focuses on predicting customer response to bank marketing campaigns (the target variable `y`) using a large-scale tabular dataset. The study was developed as part of the **Kaggle Playground Series - Season 5, Episode 8**. 

### 🚀 Live Demo
Explore the prediction model here: **[Bank Marketing Prediction App](https://huggingface.co/spaces/bdaser/Bank_Marketing)**

### 📊 Dataset Overview
The dataset is comprehensive, comprising 750,000 entries in the training set and 250,000 entries in the test set. It includes 18 columns, covering demographic information like age, job, and marital status, alongside various financial history attributes.

### 🛠️ Data Preprocessing
To ensure model robustness and accuracy, the following preprocessing steps were implemented:
* **Feature Scaling**: Numerical columns were scaled using `StandardScaler`.
* **Encoding**: Categorical features (object) were processed using `OrdinalEncoder`.

### 🏆 Model Performance
Various classification algorithms were evaluated to determine the most effective approach for this dataset. The **RandomForestClassifier** outperformed other models, demonstrating the highest overall accuracy and a strong balance between precision and recall.

| Model | Accuracy | Precision | Recall | F1 |
| :--- | :--- | :--- | :--- | :--- |
| **RandomForestClassifier** | **0.930073** | **0.768926** | **0.601061** | **0.674709** |

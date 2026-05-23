# 🏦 Bank Marketing Prediction Model

This project focuses on predicting customer response to bank marketing campaigns (the target variable `y`) using a large-scale tabular dataset. The study was developed as part of the **Kaggle Playground Series - Season 5, Episode 8: Binary Classification with a Bank Dataset**. 

### 🚀 Live Demo
You can explore the prediction model here: https://huggingface.co/spaces/bdaser/Bank_Marketing

### 📊 Dataset Overview
The dataset is comprehensive, comprising 750,000 entries in the training set and 250,000 entries in the test set. It includes 18 columns, covering demographic information like age, job, and marital status, alongside various financial history attributes.

### 🛠️ Data Preprocessing
To ensure model robustness and accuracy, the following preprocessing steps were implemented:
* **Feature Scaling**: Numerical columns (int64, float64, int32) were scaled using `StandardScaler`.
* **Encoding**: Categorical features (object) were processed using `OrdinalEncoder`, with the `handle_unknown='use_encoded_value'` parameter set to manage unseen data with a `-1` label.

### 🏆 Model Performance
Various classification algorithms were evaluated to determine the most effective approach for this dataset. The **RandomForestClassifier** outperformed other models, demonstrating the highest overall accuracy and a strong balance between precision and recall.

| Model | Accuracy | Precision | Recall | F1 |
| :--- | :--- | :--- | :--- | :--- |
| **RandomForestClassifier** | **0.930073** | **0.768926** | **0.601061** | **0.674709** |

### 📈 Analysis Summary
The `RandomForestClassifier` achieved the highest performance with an accuracy of approximately 93%. The confusion matrix analysis confirms that the model is particularly effective in classifying negative outcomes, making it the most reliable choice for this marketing prediction task.

Breast Cancer Classification using Logistic Regression

📌 Project Overview

This project builds a binary classification model to predict whether a tumor is malignant (M) or benign (B) using the Wisconsin Breast Cancer dataset.

The model uses Logistic Regression trained on selected tumor features such as radius, texture, perimeter, area, smoothness, compactness, concavity, and concave points.

⸻

🎯 Objective

To apply supervised machine learning techniques to classify breast cancer cases and evaluate model performance using standard classification metrics.

⸻

📊 Dataset

* Source: Kaggle (Enhanced Breast Cancer Dataset)
* https://www.kaggle.com/datasets/shivasingh4945/enhanced-breast-cancer-diagnostic-dataset
* Number of samples: 5,500
* Target variable: diagnosis
    * M → Malignant (1)
    * B → Benign (0)

Features used:

* radius_mean
* texture_mean
* perimeter_mean
* area_mean
* smoothness_mean
* compactness_mean
* concavity_mean
* concave points_mean

Note: Engineered features were removed to avoid redundancy and leakage.

⸻

🧹 Data Preprocessing

The following preprocessing steps were applied:

* Removed irrelevant columns (ID + engineered features)
* Converted diagnosis into binary format (M = 1, B = 0)
* Fixed inconsistent data types (converted concavity_mean to float)
* Split dataset into training (80%) and testing (20%)
* Standardized features using StandardScaler

⸻

🧠 Model Used

* Algorithm: Logistic Regression
* Library: Scikit-learn
* Input: Scaled numerical features
* Output: Binary classification (0 = Benign, 1 = Malignant)

⸻

📈 Evaluation Metrics

Confusion Matrix:

* True Negatives (TN): 680
* False Positives (FP): 22
* False Negatives (FN): 49
* True Positives (TP): 349

Classification Report:

* Accuracy: 94%
* Precision (Malignant): 0.94
* Recall (Malignant): 0.88
* F1-score: 0.91

⸻

📌 Key Insights

* Logistic Regression performs well on this dataset with high accuracy.
* Feature scaling significantly improves model stability.
* Removing engineered features ensures the model learns from raw data rather than derived signals.
* Some features (e.g., radius, perimeter, area) are highly correlated.

⸻

🚀 How to Run

1. Clone this repository:

git clone https://github.com/your-username/breast-cancer-logistic-regression.git

2. Install dependencies:

pip install -r requirements.txt

3. Open notebook:

jupyter notebook

⸻

🛠️ Requirements

* Python 3.x
* numpy
* pandas
* matplotlib
* scikit-learn

⸻

📚 Future Improvements

* Try other models (Random Forest, SVM, KNN)
* Perform feature selection / PCA
* Hyperparameter tuning (GridSearchCV)
* Handle multicollinearity explicitly
* Compare model performance across algorithms

⸻

👤 Author
John Lee Yan Long
Machine Learning Project (Beginner Portfolio)

⸻

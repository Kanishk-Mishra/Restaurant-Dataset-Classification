# Marketing Strategy Personalised Offer

This repository contains my solution for the **Marketing Strategy Personalised Offer** challenge. The goal of the project is to predict whether a customer will accept a personalised offer based on their profile and behaviour.

## 🏆 Project Details
- **Competition Link:** [Marketing Strategy - Personalised Offer](https://www.kaggle.com/competitions/marketing-strategy-personalised-offer)
- **Task:** Predict whether a customer will accept a personalised offer (binary classification).
  - **Target:** "Offer Accepted" (Yes or No)
- **Dataset:**
  - **Train Set:** Contains customer data with demographic and behavioural features.
  - **Test Set:** Contains customer data for predictions.
  - [Download the dataset here](https://www.kaggle.com/competitions/marketing-strategy-personalised-offer/data)

## 🚀 Model & Approach
- **Model:** XGBoost (with hyperparameter tuning), SVC, and KNeighborsClassifier
- **Framework:** Python, scikit-learn, pandas, XGBoost
- **Data Preprocessing:**
  - Handled missing data and categorical variables (One-Hot Encoding).
  - Feature transformations for columns like `income_range`, `age`, and customer preferences (e.g., restaurant spend, cold drinks visits).
- **Feature Engineering:**
  - Converted ranges to average values (e.g., income range, number of visits).
  - Imputed missing values using the most frequent category.
- **Training Strategy:**
  - Used XGBoost for classification with hyperparameter tuning.
  - Additionally, experimented with `SVC()` (Support Vector Classifier) and `KNeighborsClassifier()` for comparison.
  - Optimized models using GridSearchCV and RandomizedSearchCV for better performance.
  - Evaluated using accuracy, but tuned for binary classification to predict customer responses.

## 📂 Repository Structure
```
|-- dataset/                # Folder containing the dataset (train and test data)
|-- LICENSE                 # The license for the project
|-- README.md               # This file
|-- notebook.ipynb          # Kaggle notebook with full code
|-- submission.csv          # Final submission file
```

## 📌 Dependencies
Make sure you have the required libraries installed:
```bash
pip install pandas numpy scikit-learn xgboost
```

## 📊 Results
- **Best Model:** XGBoost (with hyperparameter tuning)
- **Other Models Tested:**
  - Support Vector Classifier (`SVC()`)
  - KNeighbors Classifier (`KNeighborsClassifier()`)
- **Final Test Predictions:** Binary predictions (Yes or No for offer acceptance)

## 🔥 Future Improvements
- Fine-tune the XGBoost model further for optimal performance.
- Experiment with other models like RandomForest or LightGBM.
- Implement feature scaling for numerical features like `age` and `income_range` for better model performance.
- Explore advanced imputation methods for missing data.

## 🤝 Contributions & Feedback
If you have suggestions or improvements, feel free to open an issue or a pull request! 🚀

📍 Check out my Kaggle profile [here](https://www.kaggle.com/canisqmisra)

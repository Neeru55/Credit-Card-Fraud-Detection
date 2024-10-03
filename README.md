# Credit Card Fraud Detection

## Overview
This project aims to develop a machine learning model to detect fraudulent credit card transactions. The dataset used for this analysis is sourced from [insert source or link if applicable].

## Libraries Used
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Seaborn**: For data visualization.
- **Matplotlib**: For plotting graphs.
- **Scikit-learn**: For machine learning algorithms and evaluation metrics.
- **XGBoost**: For advanced boosting algorithms.
- **Imbalanced-learn**: For handling class imbalance using SMOTE.

## Dataset
The dataset contains various features related to credit card transactions. The key attributes include:
- `Amount`: The transaction amount.
- `Class`: The target variable where 0 represents non-fraudulent transactions and 1 represents fraudulent transactions.

## Data Exploration
- **Data Loading**: Loaded the dataset using Pandas.
- **Statistical Summary**: Analyzed the data structure, summary statistics, and missing values.
- **Visualizations**:
  - Class distribution of fraudulent vs. non-fraudulent transactions.
  - Distribution of transaction amounts.
  - Boxplots to identify outliers.

## Data Preprocessing
- **Normalization**: Used StandardScaler to standardize the feature values.
- **Handling Class Imbalance**: Applied SMOTE to oversample the minority class.

## Model Building
The following models were implemented:
1. **Decision Tree Classifier**
2. **XGBoost Classifier**

### Model Evaluation
The models were evaluated using the following metrics:
- **Accuracy**
- **Precision**
- **AUC-ROC**

### AUC-ROC Curve
The ROC curves for both Decision Tree and XGBoost models were plotted, illustrating the trade-off between sensitivity and specificity. The AUC values were calculated to quantify the performance of each model.

## Results
| Model              | Accuracy | Precision | AUC      |
|--------------------|----------|-----------|----------|
| Random Forest      | [ 0.999889] | [0.999778]   | [0.999888] |
| XGBoost            | [0.999801] | [0.999602]   | [0.999800] |

## Conclusion
The project successfully implemented and evaluated models to detect credit card fraud, showcasing the effectiveness of using ensemble methods like XGBoost.

## Future Work
- Explore other algorithms such as LightGBM and CatBoost.
- Investigate feature importance to identify key factors in fraud detection.

## Requirements
Make sure to install the required libraries using:
```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost imbalanced-learn
```
## Usage

Run the `credit_card_fraud_detection.py` script to execute the analysis.

## License

This project is licensed under the MIT License 

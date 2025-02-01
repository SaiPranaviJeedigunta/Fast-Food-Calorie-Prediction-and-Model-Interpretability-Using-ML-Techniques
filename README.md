# Fast Food Calorie Prediction

This project builds a machine learning pipeline to predict the calorie content of fast food items using various regression models, including OLS Regression, Random Forest, and H2O AutoML. The goal is to evaluate model performance, conduct feature analysis, and optimize predictions using automated hyperparameter tuning.

## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Data Preprocessing](#data-preprocessing)
- [Modeling Techniques](#modeling-techniques)
- [Evaluation Metrics](#evaluation-metrics)
- [SHAP Analysis](#shap-analysis)
- [How to Run](#how-to-run)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
The project leverages a dataset of fast food nutritional information to predict calorie content. Key steps include:

1. Data preprocessing, feature engineering, and handling missing values.
2. Building regression models: OLS Regression, Random Forest Regressor, and H2O AutoML.
3. Model evaluation with metrics like R², and interpretation of results using SHAP values.
4. Statistical validation using p-values, Durbin-Watson, and Jarque-Bera tests.

## Technologies Used
- Python (pandas, numpy, matplotlib, seaborn)
- Scikit-learn
- H2O AutoML
- SHAP & LIME for model interpretability

## Data Preprocessing
- Missing values were filled using mean imputation per restaurant, followed by overall mean where necessary.
- Categorical variables (e.g., restaurant names) were converted to numerical values for model compatibility.
- Statistical tests (p-values, Durbin-Watson, Jarque-Bera) were conducted to ensure model assumptions and accuracy.

## Modeling Techniques
1. **OLS Regression:** Explored relationships between features and calorie content.
2. **Random Forest Regressor:** Built tree-based models for more robust predictions.
3. **H2O AutoML:** Automated model selection and hyperparameter tuning to optimize performance.

## Evaluation Metrics
- **R² Score:** Achieved an R² of 0.976, indicating high model accuracy.
- **Feature Importance:** Identified key predictors such as cal_fat, total_carb, and protein.
- **Model Interpretation:** Used SHAP values to explain model predictions and feature impacts.

## SHAP Analysis
SHAP (SHapley Additive exPlanations) was used to interpret feature contributions in the Random Forest and AutoML models, providing insights into which features most influenced calorie predictions.

## Results
- Achieved high predictive accuracy with an R² score of 0.976.
- Identified key features affecting calorie content.
- Automated model selection using H2O AutoML led to optimal model performance.

## Contributing
Feel free to fork this repository, make enhancements, and submit pull requests. For major changes, please open an issue to discuss what you'd like to change.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

For more details, refer to the code and comments within the repository!


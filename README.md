
# Parkinson's Predictor

This project aims to predict Parkinson's disease presence using machine learning techniques. Below is an overview of the project's methodology, findings, and limitations.

## Overview
1. **Initial Approach**:  
   - Started with a **simple logistic regression model** as a baseline to understand the dataset and establish initial predictions.

2. **Feature Selection**:  
   - Used **Sequential Feature Selection (SFS)** to reduce the dimensionality of the input features \( X \).  
   - SFS iteratively selected features that improved model performance while maintaining simplicity.

3. **Cross-Validation**:  
   - Implemented **cross-validation** to assess the model's performance and reduce the risk of overfitting due to the small dataset size.

## Results
- The model achieved **good accuracy** in predicting Parkinson's disease.
- However, the **ROC-AUC score was poor**, suggesting challenges in distinguishing between classes.  
- This discrepancy was attributed to the small dataset size, which included fewer than 200 entries.

## Limitations
1. **Dataset Size**:  
   - The small number of entries limited the robustness of the model and its ability to generalize.
   
2. **Model Exploration**:  
   - Focused only on logistic regression and did not explore other machine learning algorithms (e.g., SVM, Random Forest, etc.).

3. **Feature Selection Techniques**:  
   - Sequential Feature Selection was the only method used. Other techniques like recursive feature elimination (RFE) or L1 regularization were not tried.

## Future Improvements
- Expanding the dataset to improve model training and evaluation.
- Experimenting with more advanced models and techniques, such as:
  - Support Vector Machines (SVM)
  - Random Forests
  - Gradient Boosting (e.g., XGBoost, LightGBM)
- Trying alternative feature selection methods to compare their performance against SFS.
- Performing hyperparameter optimization to fine-tune the model for better results.

## Conclusion
While the project achieved moderate success with good accuracy, the low ROC-AUC score highlights the challenges posed by the dataset's small size. Future iterations of this project will focus on overcoming these limitations to build a more reliable predictor.

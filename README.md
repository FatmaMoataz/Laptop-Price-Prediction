# Laptop Price Prediction

## Description
This project predicts laptop prices using multiple machine learning models. The dataset includes laptop specifications such as price, storage, RAM, CPU, GPU, and more.

## Models Used
- Linear Regression (baseline)
- Random Forest (best performance)
- XGBoost
- LightGBM
- Neural Network (MLPRegressor)

## Workflow
1. **Feature Selection**: Selected numeric and important categorical features (one-hot encoding applied)
2. **Data Preprocessing**: Missing value handling, scaling
3. **Model Training**: Train-test split (80-20), evaluation with RMSE, MAE, R²
4. **Hyperparameter Tuning**: RandomizedSearchCV for Random Forest
5. **Cross-Validation**: 5-fold CV applied for generalization

## Results
| Model | RMSE | R² |
|-------|------|----|
| Linear Regression | 387.76 | 0.697 |
| Random Forest | 294.03 | 0.826 |
| XGBoost | 297.45 | 0.822 |
| LightGBM | 340.68 | 0.766 |
| Neural Network | 442.83 | 0.605 |


## Conclusion
Random Forest achieved the best performance with lowest RMSE and highest R², showing good predictive power for laptop prices.

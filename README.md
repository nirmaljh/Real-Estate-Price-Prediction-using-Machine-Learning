# Real-Estate-Price-Prediction-using-Machine-Learning
# Introduction:
This project focuses on constructing and deploying a real estate price prediction model using machine learning algorithms. The primary goal is to develop an accurate predictive model capable of estimating housing prices based on various input features. The project involves data preprocessing, model training, comprehensive evaluation of the selected model for practical usage.
# Project Steps:
1. Data Exploration:
The project begins by importing the housing dataset using the Pandas library. The dataset's dimensions, attributes, and data types are thoroughly examined to gain a comprehensive understanding. Descriptive statistics and histograms are utilized to unveil data distributions and characteristics.
2. Train-Test Splitting:
The dataset is split into training and test sets to assess the model's performance. Utilizing stratified splitting ensures that crucial variables, such as 'CHAS' (proximity to a river), are represented proportionally in both sets.
3. Feature Engineering and Preprocessing:
Feature engineering involves generating the 'TAXRM' feature by calculating the tax-to-rooms ratio. Data preprocessing is executed through a pipeline that integrates missing value imputation and feature standardization using Scikit-learn's `SimpleImputer` and `StandardScaler`.
4. Model Selection and Training:
Three distinct models are chosen for training: Random Forest Regressor, Decision Tree Regressor, and Linear Regression. Each model is trained on the preprocessed training data.
5. Model Evaluation:
The models' performance is meticulously evaluated using the Mean Squared Error (MSE) and Root Mean Squared Error (RMSE) metrics. Cross-validation is employed to ensure robust evaluation, and the RMSE scores from each fold provide a comprehensive overview of the models' predictive capabilities.
6. Model Comparison and Selection:
The RMSE scores for the models are as follows:
- Random Forest Regressor: 3.29
- Linear Regression: 5.03
- Decision Tree Regressor:  5.03

Comparing the RMSE scores, the Random Forest Regressor exhibits the lowest RMSE score, indicating superior predictive accuracy.
7. Model Usage:
The chosen Random Forest Regressor model is saved using the `joblib` library, enabling its future utilization. A practical usage example showcases how the saved model can accurately predict housing prices, underscoring its value in real-world applications.
# Conclusion:
This project demonstrates the end-to-end process of developing and deploying a real estate price prediction model. By incorporating data preprocessing, meticulous model selection, and comprehensive evaluation, the Random Forest Regressor emerges as the optimal choice with the lowest RMSE score. Its superior predictive performance positions it as a valuable tool for stakeholders seeking reliable insights for informed real estate transactions.
Future Enhancements:
Subsequent iterations of this project could explore advanced feature engineering, fine-tuning of hyperparameters, and the integration of ensemble techniques to further elevate the model's predictive accuracy. Moreover, creating user-friendly applications or platforms incorporating the model could extend its utility within the real estate domain, offering users precise and actionable price predictions.

# Concrete Compressive Strength Prediction

This project predicts the compressive strength of concrete based on its ingredients using a machine learning model. It leverages the **Concrete Compressive Strength Dataset** from the UCI Machine Learning Repository and implements data preprocessing, visualization, and predictive modeling with a Random Forest Regressor.

## Project Structure
- `concrete_strength_prediction.ipynb`: The main notebook containing step-by-step code.
- `requirements.txt`: List of dependencies required to run the project.
- `README.md`: Project documentation (this file).

## Dataset
The dataset contains 1030 instances with the following features:
- Cement (kg in a cubic meter)
- Blast Furnace Slag (kg in a cubic meter)
- Fly Ash (kg in a cubic meter)
- Water (kg in a cubic meter)
- Superplasticizer (kg in a cubic meter)
- Coarse Aggregate (kg in a cubic meter)
- Fine Aggregate (kg in a cubic meter)
- Age (days): Age of the concrete in days
- **Compressive Strength (MPa)** (Target): The output variable representing concrete strength.

You can download the dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength).

## Workflow
1. **Data Preprocessing**:
   - Load the dataset and handle missing values.
   - Rename columns for better readability.
   - Perform feature scaling using StandardScaler.

2. **Data Visualization**:
   - Correlation heatmap to identify relationships between features and the target variable.
   - Scatter plots for exploratory data analysis.

3. **Modeling**:
   - Train-Test split (80-20 ratio).
   - Train a Random Forest Regressor.
   - Evaluate the model using metrics such as Mean Squared Error (MSE) and R² Score.

4. **Visualization of Results**:
   - Plot Actual vs Predicted Compressive Strength.

5. **Model Saving**:
   - Save the trained model using `joblib` for future use.

# Predictive Maintenance Project

This project is part of the **DEPI Scholarship** initiative and focuses on utilizing machine learning techniques to predict machine failures and enhance maintenance efficiency. By leveraging historical data and predictive analytics, this project aims to reduce unplanned downtime and optimize industrial processes.

## Subject: Predictive Maintenance Using Machine Learning

### Objective:
The goal of this project is to develop and evaluate machine learning models to predict potential machine failures based on operational data. This allows for proactive maintenance, minimizing disruptions and improving operational efficiency.

### Dataset:
- **File Name:** `predictive_maintenance.csv`
- **Description:** The dataset includes features such as air temperature, process temperature, rotational speed, torque, tool wear, and machine type.
- **Target Column:** `Target` (Indicates failure or non-failure of the machine)

### Key Features:
- `Air temperature [K]`
- `Process temperature [K]`
- `Rotational speed [rpm]`
- `Torque [Nm]`
- `Tool wear [min]`
- `Type` (Categorical: L, M, H)

### Steps and Methodology:

1. **Data Preprocessing:**
   - Handled missing values and checked for data imbalances.
   - Applied one-hot encoding to categorical data (`Type`).
   - Used SMOTE to address class imbalance in the target variable.

2. **Exploratory Data Analysis (EDA):**
   - Visualized feature correlations using heatmaps.
   - Analyzed failure distribution across machine types.

3. **Model Training:**
   - Experimented with multiple machine learning models:
     - Logistic Regression
     - Decision Tree Classifier
     - Random Forest Classifier
     - Support Vector Machine (SVM)
   - Evaluated model performance using accuracy and classification reports.

4. **Hyperparameter Tuning:**
   - Tuned the Random Forest Classifier to improve accuracy and performance.

5. **Model Evaluation:**
   - Final model accuracy: **Tuned Random Forest Classifier** achieved superior performance.
   - Saved the trained model for future use.

### Results:
- **Best Model:** Random Forest Classifier
- **Accuracy:**  ≥ 90% (after hyperparameter tuning)
- Detailed classification reports are included for all models.

### How to Use:
1. Clone this repository.
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Load the saved model (`random_forest_final.pkl`) to make predictions on new data.

### Visualizations:
The project includes insightful visualizations such as:
- Correlation heatmaps
- Target variable distribution
- Machine type-specific failure distributions

### Future Enhancements:
- Integrate real-time data streaming for predictive maintenance.
- Explore additional machine learning algorithms like Gradient Boosting or Neural Networks.
- Deploy the model as a web service for operational use.

### Acknowledgments:
This project is supported by the **DEPI Scholarship** program. Special thanks to mentors and peers for their guidance and collaboration.

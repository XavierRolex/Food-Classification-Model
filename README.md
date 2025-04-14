# Food Classification Model

## Overview
This project involves building a machine learning model to classify food items as either **healthy** or **unhealthy** based on various features. The classification task is performed using multiple machine learning algorithms, including Logistic Regression and Decision Tree Classifier. The project also includes hyperparameter tuning and model evaluation using cross-validation techniques to optimize the model's performance.

## Project Workflow

1. **Data Preprocessing**: 
   - Outlier removal using IQR.
   - Handling missing values (drop columns with >50% missing data, impute others).
   - Encoding categorical features using OneHotEncoder.
   - Scaling the features using StandardScaler.

2. **Model Training**:
   - Logistic Regression.
   - Decision Tree Classifier.
   - Hyperparameter tuning using GridSearchCV.

3. **Model Evaluation**:
   - Accuracy, Precision, Recall, F1 Score.
   - Confusion Matrix to assess model performance.
   - Cross-validation to ensure model generalization.

4. **Learning Curves and Validation Curves**:
   - Learning Curve to visualize the model's training performance.
   - Validation Curve for hyperparameter tuning to find the optimal model settings.

## Requirements
- Python 3.x
- scikit-learn
- pandas
- numpy
- seaborn
- matplotlib

You can install the required dependencies by running the following command:

```bash
pip install -r requirements.txt

├── data/
│   └── food_data.csv               # Dataset file
├── notebooks/
│   └── preprocessing.ipynb         # Jupyter notebook for data preprocessing
├── src/
│   ├── create_database.py          # Script for creating the database
│   ├── chatbot.py                  # Chatbot implementation
│   └── model.py                    # Model training and evaluation
├── requirements.txt                # List of project dependencies
├── README.md                       # Project documentation

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
```

```bash
File Structure
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
```

## Model Evaluation

The models were evaluated using the following metrics:
- **Accuracy**: Measures the percentage of correct predictions.
- **Precision**: Measures the proportion of positive predictions that are actually correct.
- **Recall**: Measures the proportion of actual positive instances that were correctly predicted.
- **F1 Score**: A weighted average of Precision and Recall.

### Logistic Regression Results:
- **Accuracy**: `0.XX`
- **Precision**: `0.XX`
- **Recall**: `0.XX`
- **F1 Score**: `0.XX`

### Decision Tree Classifier Results:
- **Accuracy**: `0.XX`
- **Precision**: `0.XX`
- **Recall**: `0.XX`
- **F1 Score**: `0.XX`

## Hyperparameter Tuning

- **Logistic Regression**: 
  - Hyperparameters tuned include regularization strength (`C`), solver, and maximum iterations.
  
- **Decision Tree Classifier**: 
  - Hyperparameters tuned include `max_depth`, `min_samples_split`, `min_samples_leaf`, and `ccp_alpha`.

## Cross-Validation

Cross-validation was performed for both models using 5-fold cross-validation to ensure the robustness of the models and prevent overfitting.

## Learning Curves

Learning curves were plotted to show the relationship between the training set size and model performance. The curves help in diagnosing whether the model is underfitting or overfitting.

## Validation Curves

Validation curves were plotted to assess how changes in model hyperparameters, specifically the maximum depth of the Decision Tree, affect model performance.

## How to Run the Project

1. **Clone the Repository:**

```bash
git clone https://github.com/yourusername/food-classification.git
cd food-classification
```

2. **Install Dependencies:**
```bash
   pip install -r requirements.txt
```

3. **Run the Model Evaluation:**
```bash
python classification_of_food.py
```
4.   **View Results:**
   - Check the console output for evaluation metrics such as accuracy, precision, recall, and F1 score.
   - The confusion matrices for both models will also be displayed.
       
## Contributing
Feel free to fork this repository, submit issues, or create pull requests. If you wish to contribute, please fork the repository and make changes in your branch. Once you're ready, submit a pull request for review.

## License 
This project is licensed under the MIT License - see the LICENSE file for details.


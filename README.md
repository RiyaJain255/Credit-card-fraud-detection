# Credit Card Fraud Detection

This repository presents a machine learning approach to detect fraudulent credit card transactions. The project utilizes various classification algorithms and addresses the challenge of imbalanced datasets common in fraud detection.

## Dataset

The project uses a dataset containing credit card transactions, including features like time, amount, and anonymized features (V1-V28), and a 'Class' label indicating fraudulent or legitimate transactions.

## Project Structure

-   `credit_card_dataset.csv`: The dataset file (or a placeholder for its location).
-   `credit_card_fraud_detection.ipynb`: The Jupyter notebook containing the code for data preprocessing, model training, and evaluation.

## Dependencies

The following libraries are required to run the notebook:

-   pandas
-   numpy
-   matplotlib
-   seaborn
-   scikit-learn
-   imblearn

## Methodology
The project follows these steps:

Data Loading and Initial Exploration: Loading the dataset and performing initial data exploration (though not explicitly shown in the provided notebook, it's a standard first step).
## Data Preprocessing:
-Feature Scaling: Scaling the 'Amount' feature using StandardScaler.

-Handling Missing Values: Imputing missing values in the features using SimpleImputer with a mean strategy.

-Handling Class Imbalance: Applying the Synthetic Minority Over-sampling Technique (SMOTE) to the training data to address the imbalance between fraudulent and non-fraudulent transactions.

-Model Training: Training several classification models:
  --Logistic Regression
  --Random Forest Classifier
  --Gradient Boosting Classifier
  --Support Vector Machine (SVC)
  --Neural Network (MLPClassifier)
  
-Model Evaluation: Evaluating the performance of each model using the following metrics:
  --Area Under the Precision-Recall Curve (AUPRC)
  --Confusion Matrix
  --Accuracy Score
  --Precision Score
  --F1-score
  
-Results
The notebook includes the AUPRC, Confusion Matrix, Accuracy, Precision, and F1-score for each trained model on the test set. Visualizations of the Precision-Recall Curve and Confusion Matrix are also generated to help assess model performance, especially in the context of imbalanced data.

You can install these dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imblearn


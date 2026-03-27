# Telecom Customer Churn Prediction using Feedforward ANN

This project predicts customer churn using a feedforward Artificial Neural Network (ANN) on the Telco Customer Churn dataset. The main goal of the project is to identify whether a customer is likely to leave the telecom service based on customer demographics, account details, service usage, and billing information.

## Project Objective

The objective of this project is to:
- Understand customer churn behavior using data analysis.
- Preprocess the telecom dataset properly for model building.
- Build a simple feedforward ANN model for binary classification.
- Evaluate the model using suitable classification metrics.
- Suggest business actions based on the results.

## Dataset

The dataset used in this project is the **Telco Customer Churn Dataset**.  
It contains customer-related information such as:
- Gender
- Senior citizen status
- Partner and dependents
- Tenure
- Phone and internet services
- Online security, backup, tech support
- Contract type
- Payment method
- Monthly charges
- Total charges
- Churn status

## Project Workflow

The project follows these steps:
1. Data loading and understanding
2. Data cleaning and preprocessing
3. Exploratory Data Analysis (EDA)
4. Feature encoding and scaling
5. Train-test split
6. Building the feedforward ANN model
7. Model evaluation using accuracy, precision, recall, F1-score, and confusion matrix
8. Business interpretation of results

## Model Used

The model used in this project is a **Feedforward Artificial Neural Network** built using `MLPClassifier`.

### Model configuration
- Hidden layers: `(16, 8)`
- Activation function: `ReLU`
- Optimizer: `Adam`
- Early stopping: Enabled
- Maximum iterations: `300`

## Results

The ANN model achieved:
- Accuracy: **80%**
- Better performance on non-churn customers than churn customers
- Churn class recall: **49%**

This means the model performs reasonably well overall, but it still misses some actual churn cases.

## Files in this Repository

- `surendra_prasad_ANN_assignment.ipynb` - Main notebook containing complete code and analysis
- `telco_churn.csv` - Dataset used in the project
- `Telco_Churn_Data_Dictionary.pdf` - Original data dictionary
- `Updated_Telco_Churn_Data_Dictionary.xlsx` - Updated data dictionary after preprocessing
- `2025em1100109_ANN_report.docx` - Final report
- `README.md` - Project documentation

## Installation and Requirements

To run this project, install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run

1. Clone this repository:
```bash
git clone https://github.com/SurendraPrasadSH/Telecomm_churn-using-ANN_feetForward.git
```

2. Open the project folder:
```bash
cd Telecomm_churn-using-ANN_feetForward
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

4. Open the notebook file and run all cells.

## Evaluation Metrics

The model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Training Loss Curve

## Business Insights

Some important insights from the project:
- Customers with month-to-month contracts are more likely to churn.
- Customers with lower tenure are more likely to leave.
- Internet service type and monthly charges also affect churn behavior.

## Future Improvements

Possible improvements for this project:
- Handle class imbalance more effectively
- Try hyperparameter tuning
- Compare ANN with other machine learning models
- Improve churn recall using resampling or threshold tuning

## Author

**Surendra Prasad**  
BITS Pilani

## Note

This project was developed for academic purposes as part of an assignment on Artificial Neural Networks.

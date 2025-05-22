# Insurance-Fraud-Detection
This project uses Python and XGBoost to analyze insurance claims data and predict the likelihood of fraud.

## Description

This project develops a machine learning model to predict insurance fraud using claims data. The project includes data cleaning and preprocessing, exploratory data analysis (EDA), model building with XGBoost, hyperparameter tuning, and feature importance analysis. The goal is to identify fraudulent claims and provide insights for insurance companies to minimize financial losses.

## Dataset

The dataset used in this project is `insurance_data.csv`. It contains information about insurance claims, including customer details, policy information, incident reports, and claim amounts.

* **Source:** The dataset is available on GitHub at: [https://github.com/simranjeet97/Top-Machine-Learning-Algorithms-Python/blob/main/insurance_data.csv](https://github.com/simranjeet97/Top-Machine-Learning-Algorithms-Python/blob/main/insurance_data.csv)

## Installation

1.  Clone the repository:

    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/KrittikaDas/Insurance-Fraud-Detection.git) 
    cd Insurance-Fraud-Detection
    ```

2.  It is recommended to use a virtual environment:

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Linux/macOS
    venv\Scripts\activate  # On Windows
    ```

3.  Install the required Python packages:

    ```bash
    pip install pandas scikit-learn seaborn matplotlib imblearn xgboost
    ```

## Usage

1.  Open the Jupyter Notebook `insurance_fraud_detection.ipynb` in your Jupyter environment (e.g., Jupyter Notebook, JupyterLab, or Google Colab).

    ```bash
    jupyter notebook insurance_fraud_detection.ipynb
    ```

2.  Run the cells sequentially to execute the data analysis and model building steps.

## Results

The key results of this project include:

* An XGBoost model was trained and tuned to predict insurance fraud.
* Hyperparameter tuning using RandomizedSearchCV improved the model's performance.
* Feature importance analysis identified key predictors of fraud, such as:
    * `collision_type_Unknown`
    * `insured_hobbies_chess` and `insured_hobbies_cross-fit`
    * Specific `policy_bind_date` values
    * `incident_severity_Total Loss` and `incident_severity_Minor Damage`
* Feature selection (using the top 20 features) further improved the model's ROC AUC score on the test set to 0.847 and significantly increased recall for the fraud class.
* A business recommendation summary was generated, providing actionable insights for the insurance company.

## Files

* `insurance_fraud_detection.ipynb`: Jupyter Notebook containing the code for data loading, cleaning, EDA, model building, and evaluation.
* `insurance_data.csv`: The dataset used for the project.
* `README.md`: This file.

## Author

Krittika Das

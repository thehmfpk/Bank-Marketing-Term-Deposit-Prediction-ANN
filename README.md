# Bank Marketing Term Deposit Prediction using ANN

## Project Overview
This project aims to predict the success of a bank marketing campaign. The goal is to determine whether a client will subscribe to a term deposit (target variable `y`) based on various features such as age, job, marital status, and previous campaign outcomes. 

We utilize an **Artificial Neural Network (ANN)** built with TensorFlow/Keras to perform this binary classification task.

## Dataset Information
The project uses the **Bank Marketing Dataset** (commonly found on the UCI Machine Learning Repository).
- **Total Records:** 45,211
- **Features:** 16 independent variables (Categorical and Numerical)
- **Target Variable:** `y` (binary: 'yes', 'no')

### Key Features:
- **Customer Profile:** Age, Job, Marital Status, Education, Default, Balance, Housing, Loan.
- **Campaign Data:** Contact type, Day, Month, Duration, Campaign (number of contacts).
- **Previous Contact:** Pdays, Previous, Poutcome.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:**
  - Data Processing: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Machine Learning: `scikit-learn`
  - Deep Learning: `tensorflow`, `keras`

## 🚀 Project Workflow
1. **Data Loading & Exploration (EDA):** Understanding data distributions and checking for missing values.
2. **Preprocessing:**
   - Encoding categorical variables using `LabelEncoder`.
   - Feature scaling using `StandardScaler`.
   - Splitting data into Training and Testing sets.
3. **Model Architecture:**
   - **Input Layer:** 64 units, ReLU activation, Dropout (0.3).
   - **Hidden Layer 1:** 32 units, ReLU activation, Dropout (0.3).
   - **Hidden Layer 2:** 16 units, ReLU activation.
   - **Output Layer:** 1 unit, Sigmoid activation (for binary classification).
4. **Training:** Compiled with `adam` optimizer and `binary_crossentropy` loss.
5. **Evaluation:** Assessing performance using Accuracy, Confusion Matrix, and Classification Report.

## 📈 Results
The model achieved an accuracy of approximately **89.7%** on the test set.

**Classification Report Summary:**
- **Accuracy:** ~90%

The Confusion Matrix shows strong performance in predicting "No Subscription" cases, while highlighting the inherent challenge of predicting the minority "Yes" class in an imbalanced dataset.

## 📁 Repository Structure
```text
├── ANN_Bank_Marketing_Full_analysis_ML.ipynb  # Main Jupyter Notebook
├── bank-full.csv                              # Dataset file
└── README.md                                  # Project documentation
└── LICENSE                                  

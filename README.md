# Credit Scoring Prediction using Machine Learning
This project predicts the likelihood of a person defaulting on their credit payment within 2 years using machine learning model.

# Project Overview
The model predicts **credit default risk** (SeriousDlqin2yrs = 1) based on customer financial data such as:
- Age  
- Debt Ratio  
- Number of past due payments (30–59, 60–89, 90+ days)  
- Number of Dependents  

The pipeline includes:
1. Data preprocessing and cleaning  
2. Exploratory Data Analysis (EDA)  
3. Feature scaling using `StandardScaler`  
4. Model training with:
   - Logistic Regression  
   - Decision Tree  
   - Random Forest  
5. Model evaluation using ROC-AUC  
6. Interactive interface using **Gradio**

# Dataset
The dataset used is `credit_scoring_sample.csv`.  
Make sure this file is present in your working directory.

# Installation

Clone this repository and install dependencies:
'```bash'
git clone https://github.com/yourusername/credit-scoring-ml.git
cd credit-scoring-ml
pip install -r requirements.txt

# Main Files
File	Description
credit_scoring_sample.csv	Input dataset
credit_scoring_model.py	Model training and evaluation script
best_credit_model.pkl	Saved trained model
scaler.pkl	Saved scaler
app.py	Gradio interface for real-time prediction
README.md	Project documentation
# How to Run
1) Train the model
python credit_scoring_model.py
This trains the models and saves the best one (best_credit_model.pkl).

2) Launch Gradio interface
python app.py
Then open the local URL shown in your terminal to test predictions interactively.

🖥️ Gradio App Preview

Input customer details such as age, debt ratio, and number of late payments to get:

Predicted risk (Low / High)

Probability of default

📈 Example Output
✅ Low Risk of Default
Probability of default: 0.18

🧰 Technologies Used

1) Python 🐍
2) Pandas, NumPy
3) Scikit-learn
4) Seaborn, Matplotlib
5) Gradio

# Output
![3](https://github.com/user-attachments/assets/1fa04c41-28ab-4924-8aae-eb6a20424abc)

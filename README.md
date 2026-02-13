.

📊 Customer Churn Prediction using Deep Learning
📌 Project Overview

This project predicts customer churn (whether a customer will leave or stay) using a Deep Learning model (ANN) built with TensorFlow and deployed using Streamlit.

The application allows users to enter customer details and instantly get the churn probability.

🎯 Objective

Predict customer churn using customer information.

Help businesses identify customers at risk of leaving.

Demonstrate ML model deployment using Streamlit.

🧠 Technologies Used

Python

TensorFlow / Keras

Scikit-learn

Pandas & NumPy

Streamlit

Pickle

📂 Project Structure
DL/
│
├── app.py                          # Streamlit web app
├── model.h5                        # Trained ANN model
├── Churn_Modelling.csv             # Dataset
├── scaler.pkl                      # Feature scaler
├── label_encoder_gender.pkl        # Label Encoder
├── onehot_encoder_geo.pkl          # One-Hot Encoder
│
├── experiments.ipynb               # Model experimentation
├── prediction.ipynb                # Prediction testing
├── hyperparametertuningann.ipynb   # Hyperparameter tuning
├── salaryregression.ipynb          # Practice notebook
│
├── requirements.txt                # Dependencies
│
├── logs/                           # Training logs
├── regressionlogs/                 # Regression logs
└── venv/                           # Virtual environment

🔍 Features

✔️ Interactive Streamlit UI
✔️ Real-time churn prediction
✔️ Preprocessing using encoders & scaler
✔️ Deep learning model (ANN)
✔️ Probability-based output

📊 Input Features

The model predicts churn based on:

Credit Score

Geography

Gender

Age

Tenure

Balance

Number of Products

Has Credit Card

Is Active Member

Estimated Salary

⚙️ Workflow

1️⃣ Load trained model (model.h5)

2️⃣ Load preprocessing files:

Label Encoder

OneHot Encoder

Standard Scaler

3️⃣ Take user input from Streamlit UI

4️⃣ Apply:

Encoding

Scaling

5️⃣ Predict churn probability using ANN model

6️⃣ Display result to user.

🚀 Installation & Setup
Step 1 — Clone Project
git clone https://github.com/tarun-1313/Customer-Churn-Prediction
cd DL

Step 2 — Create Virtual Environment (Optional)
conda create --name churn_env python=3.10
conda activate churn_env

Step 3 — Install Dependencies
pip install -r requirements.txt

Step 4 — Run Streamlit App
python -m streamlit run app.py

📈 Sample Output
Churn Probability: 0.81
The customer is likely to churn.

🧩 Model Details

Model Type: Artificial Neural Network (ANN)

Framework: TensorFlow / Keras

Problem Type: Binary Classification

Output: Probability (0–1)

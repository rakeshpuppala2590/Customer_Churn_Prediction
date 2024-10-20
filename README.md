# 📊 Customer Churn Prediction Project

This project predicts customer churn for a bank using multiple machine learning models, with a focus on interpreting predictions and generating personalized customer communication.

---

## 🚀 Features

- **Churn Prediction Models**: The project utilizes several machine learning models for predicting customer churn:
  - `XGBoost`
  - `K-Nearest Neighbors (KNN)`
  - `Random Forest`
  - `Voting Classifier (ensemble model)`

- **Web Interface**: A user-friendly interface built with **Streamlit** allows you to:
  - Select customers from a dataset
  - Input or modify customer features (credit score, age, balance, etc.)
  - Generate predictions with the option to visualize model probabilities

- **Explainable AI**: Explanations of the prediction are generated using **OpenAI API**. These explanations are based on the customer's details and the most important features contributing to churn risk.

- **Customer Communication**: The system can generate a personalized email based on the churn prediction, offering incentives or retention strategies.

---

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/churn-prediction.git
   cd churn-prediction

2. **Install the required dependencies**:

```bash
Copy code
pip install -r requirements.txt

3. **Set your OpenAI API key in your environment variables**:

```bash
Copy code
export GROQ_API_KEY='your-api-key-here'
Ensure you have the necessary model files (e.g., xgb_model.pkl, rf_model.pkl) in the project directory. If they are not available, you can either train your models using the code provided or upload pre-trained models.



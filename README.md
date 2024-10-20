Customer Churn Prediction Project
This project predicts customer churn for a bank using multiple machine learning models, with a focus on interpreting predictions and generating personalized customer communication.

Features
Churn Prediction Models: The project utilizes several machine learning models for predicting customer churn:

XGBoost
K-Nearest Neighbors (KNN)
Random Forest
Voting Classifier (ensemble model)
Web Interface: A user-friendly interface built with Streamlit allows you to:

Select customers from a dataset
Input or modify customer features (credit score, age, balance, etc.)
Generate predictions with the option to visualize model probabilities
Explainable AI: Explanations of the prediction are generated using OpenAI API. These explanations are based on the customer's details and the most important features contributing to churn risk.

Customer Communication: The system can generate a personalized email based on the churn prediction, offering incentives or retention strategies.

Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/churn-prediction.git
cd churn-prediction
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Place your OpenAI API key in your environment variables:

bash
Copy code
export GROQ_API_KEY='your-api-key-here'
Ensure you have the necessary model files (e.g., xgb_model.pkl, rf_model.pkl) in the project directory. If they are not available, you can either train your models using the code provided or upload pre-trained models.

Running the Application
Start the Streamlit web application:

bash
Copy code
streamlit run app.py
Open the application in your browser (usually at http://localhost:8501).

How It Works
Data Input: The application allows you to input customer data, such as credit score, age, and location, or select a customer from the sample dataset.

Model Predictions: After entering the information, the app uses various machine learning models to predict the probability of churn. Model probabilities and an average probability are displayed.

Visualizations:

A gauge chart shows the overall probability of churn.
A bar chart shows the churn probability predicted by each model.
Explanations: The application uses the OpenAI API to generate a natural language explanation of the prediction, based on the most important features of the model.

Customer Email Generation: If the customer is at high risk of churning, the system generates an email offering personalized retention strategies and incentives.

Project Structure
app.py: The main Streamlit application.
utils.py: Utility functions for creating visualizations and preparing input data.
models/: Directory containing the pre-trained machine learning models.
data/: Directory for storing the dataset.
README.md: This file.
Example Usage
Select a customer from the dropdown.
Adjust features like Credit Score, Age, Balance, etc.
View the churn prediction and explanation.
Review the email generated for the customer to encourage them to stay with the bank.

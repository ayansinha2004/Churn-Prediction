📊 Customer Churn Prediction Web App

A Machine Learning based web application that predicts whether a telecom customer is likely to churn using multiple classification algorithms.

Built using Python, Scikit-learn, XGBoost, and Streamlit.

🚀 Project Overview

Customer churn prediction helps telecom companies identify customers who are likely to stop using their services.

This project:

Preprocesses customer data

Trains multiple ML models

Handles class imbalance using SMOTE

Compares model performance

Deploys a real-time prediction web app using Streamlit

🧠 Machine Learning Models Used
models = {
    "Decision Tree": DecisionTreeClassifier(random_state=42),
    "Random Forest": RandomForestClassifier(random_state=42),
    "XGBoost": XGBClassifier(random_state=42)
}
📈 Model Performance (Cross Validation Accuracy)
Model	Accuracy
Decision Tree	~77%
Random Forest	~84%
XGBoost	~83%

Final selected model: Random Forest

Test Accuracy: ~78%

📂 Dataset Information

Total Records: 7043

Features: 19

Target Variable: Churn (Yes/No)

Source: Telco Customer Churn Dataset

🛠 Data Preprocessing Steps

Removed customerID

Handled missing values in TotalCharges

Converted TotalCharges to float

Label Encoding for categorical variables

Handled class imbalance using SMOTE

Train/Test split (80/20)

💻 Streamlit Web Application Features

Clean interactive UI

User input form for customer details

Model selection option

Real-time churn prediction

Probability score display

Feature importance visualization

Example Output:
Prediction: Churn
Prediction Probability: 0.87
📦 Project Structure
customer-churn-prediction/
│
├── app.py
├── customer_churn_model.pkl
├── encoders.pkl
├── requirements.txt
└── README.md
🔧 Installation (Run Locally)
1️⃣ Clone Repository
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Run Streamlit App
streamlit run app.py
🌐 Deployment

The application can be deployed using:

Streamlit Cloud

Render

Heroku (with Docker)

AWS / GCP

📊 Business Impact

This system can help telecom companies:

Identify high-risk customers

Reduce churn rate

Improve retention strategies

Increase customer lifetime value

🔮 Future Improvements

Add SHAP explainability

Hyperparameter tuning

Model performance comparison dashboard

API deployment with FastAPI

Database integration

👨‍💻 Author

Ayan Sinha
Machine Learning & AI Enthusiast

⭐ Support

If you like this project, consider giving it a ⭐ on GitHub.

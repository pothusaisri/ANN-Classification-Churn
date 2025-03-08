# 🚀 Customer Churn Prediction Web Application 

A Streamlit-based web application for predicting customer churn probability using a pre-trained TensorFlow neural network model.

## 🌟 Features
- **📝 User Input Fields**: 
  - 🌍 Geography (France/Spain/Germany)
  - 👫 Gender (Male/Female)
  - 🎂 Age (18-92)
  - 💰 Balance & Estimated Salary
  - 📊 Credit Score (300-850)
  - ⏳ Tenure (0-10 years)
  - 🛍️ Number of Products (1-4)
  - 💳 Credit Card Ownership
  - 🔔 Active Membership Status
- **⚡ Real-time Prediction**: Instant churn probability calculation
- **🚨 Threshold Alert**: Clear indication of churn likelihood (threshold = 0.5)

## 🛠️ Installation
1. Clone the repository
   ```bash
   git clone [your-repository-url]
   ```
2. Install requirements
``` bash
  pip install -r requirements.txt
```

## 🖥️ Usage

- Place required files in project root:

model.h5 (pre-trained TensorFlow model)
label_encoder_gender.pkl
onehot_encoder_geo.pkl
scaler.pkl

- Run the application:

``` bash
streamlit run app.py
```

## Fill in customer details through the web interface

- View prediction results:

📈 Churn probability percentage

✅❌ Binary churn classification

🧠 Data Preprocessing
The application automatically handles feature engineering:

🔡 Categorical Encoding:

🏷️ Label Encoding for Gender (Male/Female → 0/1)

🔢 One-Hot Encoding for Geography (3 countries → 3 binary features)

📏 Feature Scaling:

⚖️ StandardScaler applied to all features

## 📂 Project Structure
.
├── app.py               # Main application code
├── model.h5             # 🧠 Trained neural network model
├── label_encoder_gender.pkl
├── onehot_encoder_geo.pkl
├── scaler.pkl
├── README.md
└── requirements.txt

# DeepCSAT-Ecommerce-Customer-Satisfaction-Score-Prediction
🧠 DeepCSAT – Ecommerce Customer Satisfaction Score Prediction
Welcome to DeepCSAT, a deep learning-based project that predicts Customer Satisfaction Scores (CSAT) for eCommerce support interactions. This project leverages neural networks to analyze customer support data and classify satisfaction levels from 0 (low) to 5 (high).

📌 Project Objective
To build and evaluate deep learning models capable of accurately predicting customer satisfaction based on interaction-related features, helping businesses:

Improve customer retention

Allocate resources effectively

Enhance customer support quality

🗃️ Dataset
Source: Internal / Proprietary Dataset (eCommerce_Customer_support_data.csv)

Target Variable: CSAT_Score (Categorical: 0 to 5)

Features: Various numerical and categorical columns representing support interactions (e.g., time taken, agent ID, resolution status, etc.)

⚙️ Project Structure
Copy
Edit
📁 DeepCSAT/
├── 📄 README.md
├── 📊 eCommerce_Customer_support_data.csv
├── 📓 DeepCSAT_Prediction.ipynb
├── 📁 models/
│   └── DeepCSAT_Best_Model.h5
├── 📈 results/
│   └── evaluation_metrics.png
└── 📑 requirements.txt
🧪 Models Implemented
We evaluated and compared the performance of the following models:

✅ Basic ANN

✅ ANN with Dropout

✅ ANN with Batch Normalization

✅ ANN with Dropout + BatchNormalization + L2 Regularization (Final Model)

All models were evaluated using:

Accuracy

Precision, Recall, F1-Score

Confusion Matrix

🏆 Final Model: ANN + Dropout + BatchNormalization + Regularization
Architecture:
Input → Dense(256) + BN + Dropout(0.3)

→ Dense(128) + BN + Dropout(0.3)

→ Dense(64) + BN + Dropout(0.2)

→ Output (Softmax)

Performance:
✅ Test Accuracy: ~X.XXX

✅ Balanced performance across all CSAT levels

✅ Generalizes well with minimal overfitting due to regularization

📊 Evaluation Results

Metric	Value
Accuracy	X.XX
Precision	X.XX
Recall	X.XX
F1-Score	X.XX
Confusion matrix and classification report visualized using Seaborn.

🔍 Model Explainability
We recommend using:

SHAP for feature importance

LIME for local explanations (optional)



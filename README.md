Breast Cancer Detection using Machine Learning

This project uses Machine Learning to detect breast cancer based on clinical cell measurements.
It applies Logistic Regression to classify tumors as malignant (cancerous) or benign (non-cancerous).
The model is deployed using Streamlit to provide an interactive and easy-to-use web interface for testing and awareness.

---

Overview
This project demonstrates a complete ML pipeline — from dataset loading, training, and evaluation to deployment through a Streamlit web app.
The dataset used is the Breast Cancer Wisconsin dataset (included in scikit-learn), containing 30 biological features such as cell radius, texture, smoothness, compactness, and symmetry.

The model predicts tumor type and provides a confidence score with visual progress indicators and safe/risky range hints.

---

Features

* Interactive web app for prediction
* Confidence-based interpretation and color-coded output
* Educational explanation of how AI detects cancer patterns
* Logistic Regression model trained on the Breast Cancer Wisconsin dataset
* Streamlit + Pyngrok for public deployment

---

Tech Stack
Programming Language: Python 3
Libraries: scikit-learn, pandas, streamlit, joblib, pyngrok, numpy
Algorithm: Logistic Regression
Deployment: Streamlit web app with ngrok tunneling
Model Saving: joblib and pickle

---

Project Structure

breast-cancer-detection-ml
│
├── breast_cancer_notebook.ipynb     (Model training notebook)
├── app.py                           (Streamlit prediction app)
├── breast_cancer_model.pkl          (Trained Logistic Regression model)
├── scaler.pkl                       (Saved StandardScaler)
├── requirements.txt                 (Dependencies)
└── README.md                        (Project documentation)

---

Installation and Running

Step 1 — Clone the Repository

Step 2 — Install Dependencies
pip install -r requirements.txt

Step 3 — Run the Streamlit App
streamlit run app.py

Step 4 — (Optional) Host Publicly with Ngrok
from pyngrok import ngrok
ngrok.connect(8501)

---

Model Details
Dataset: Breast Cancer Wisconsin Dataset
Algorithm: Logistic Regression
Features: 30 numeric input measurements from cell nuclei
Target Variable: Diagnosis (Benign = 1, Malignant = 0)
Evaluation Metrics: Accuracy, Classification Report

---

Example Output

User Input:
Mean Radius = 14.5
Mean Texture = 21.0
Mean Smoothness = 0.1

Output:
Prediction: Benign (Non-cancerous)
Confidence: 91%
Interpretation: Safe range, likely non-invasive cell structure.


Future Improvements

* Add image-based tumor detection using CNNs
* Deploy to Streamlit Cloud or Hugging Face Spaces
* Integrate dataset visualization dashboard
* Build an API endpoint for prediction requests



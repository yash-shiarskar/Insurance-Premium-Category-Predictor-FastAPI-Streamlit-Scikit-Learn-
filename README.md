# Insurance-Premium-Category-Predictor-FastAPI-Streamlit-Scikit-Learn-
A Machine Learning–powered web application that predicts an insurance premium category based on user attributes such as age, BMI, lifestyle risk, income, occupation, and city tier. Built using FastAPI for the backend and Streamlit for the frontend.


A Machine Learning–powered web application that predicts an insurance premium category based on user attributes such as age, BMI, lifestyle risk, income, occupation, and city tier. Built using FastAPI for the backend and Streamlit for the frontend.

✅ 📘 Full README Description (Professional Version)
🚀 Insurance Premium Category Predictor

This project is an end-to-end Machine Learning application that predicts an individual's insurance premium category based on demographic and lifestyle factors.

The system consists of:

🔹 A trained Scikit-learn model

🔹 FastAPI backend for serving predictions

🔹 Streamlit frontend for interactive user input

🔹 Pydantic validation with computed fields

🔹 Real-time prediction through REST API

🧠 Features

BMI calculation using height and weight

Lifestyle risk scoring based on BMI and smoking habits

Automatic age group classification

City tier classification (Tier 1, Tier 2, Tier 3)

REST API-based prediction system

Interactive web UI for live predictions

🏗️ Project Architecture

Frontend (Streamlit)
⬇
FastAPI Backend
⬇
Scikit-learn ML Model
⬇
Prediction Response

📂 Project Structure

app.py – FastAPI backend with model loading and prediction endpoint 

app

frontend.py – Streamlit UI for user interaction 

frontend

model.pkl – Trained ML model

fastapi_ml_model.ipynb – Model training notebook

⚙️ Tech Stack

Python

FastAPI

Streamlit

Scikit-learn

Pandas

Pydantic

▶️ How to Run Locally
1️⃣ Activate Virtual Environment
myenv\Scripts\activate
2️⃣ Start Backend
uvicorn app:app --reload
3️⃣ Start Frontend
streamlit run frontend.py

Then open:

http://localhost:8501
🎯 API Endpoint

POST /predict

Example JSON input:

{
  "age": 30,
  "weight": 70,
  "height": 1.75,
  "income_lpa": 10,
  "smoker": false,
  "city": "Mumbai",
  "occupation": "private_job"
}

Response:

{
  "predicted_category": "Low"
}

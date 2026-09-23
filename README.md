# 🏠 Property Price Forecast

A full-stack machine learning application that predicts property prices based on key features such as **property area (sq ft)** and **number of rooms**.

This project implements an end-to-end ML workflow including **data preprocessing, model training, REST API development, and interactive visualization** using Flask and Streamlit.

---

## 🚀 Features

- 🏠 Property price prediction using Machine Learning
- 🤖 Linear Regression model using Scikit-learn
- 🔥 Flask REST API backend
- 📊 Streamlit interactive user interface
- 📈 Data visualization and analysis
- 🧪 Model performance evaluation
- 🌐 API-based prediction system
- 💾 Saved trained ML model for inference

---

# 🏗️ Application Architecture

```
              User
                |
                |
        Streamlit Frontend
                |
                |
          Flask REST API
                |
                |
     Machine Learning Model
                |
                |
      Linear Regression Model
                |
                |
       Property Price Forecast
```

---

# 📂 Project Structure

```
property-price-forecast/

│
├── data/
│   └── house_price.csv              # Property dataset
│
├── model/
│   ├── model.pkl                    # Trained ML model
│   ├── scaler.pkl                   # Feature scaler
│   └── diagnostics.png              # Model evaluation plots
│
├── backend/
│   └── app.py                       # Flask REST API
│
├── frontend/
│   └── ui.py                        # Streamlit application
│
├── train_model.py                   # Model training script
│
├── requirements.txt                 # Project dependencies
│
└── README.md
```

---

# 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Language | Python |
| Machine Learning | Scikit-learn |
| ML Algorithm | Linear Regression |
| Backend | Flask |
| Frontend | Streamlit |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Plotly |
| Model Serialization | Pickle |

---

# 📊 Dataset

The model is trained using a property dataset containing:

| Feature | Description |
|---------|-------------|
| Area | Property area in square feet |
| Rooms | Number of rooms |
| Price | Target property price |

### Dataset Details

- Total Samples: 47
- Input Features: 2
- Target Variable: Property Price

Example:

| Area | Rooms | Price |
|------|-------|-------|
| 2000 sq ft | 3 | $347,820 |

---

# ⚙️ Installation & Setup

## 1. Clone Repository

```bash
git clone https://github.com/your-username/property-price-forecast.git
```

Navigate to project directory:

```bash
cd property-price-forecast
```

---

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🧠 Train Machine Learning Model

Run:

```bash
python train_model.py
```

The training script performs:

- Dataset loading
- Data preprocessing
- Feature scaling
- Model training
- Model evaluation
- Model saving

Generated files:

```
model/
├── model.pkl
└── scaler.pkl
```

---

# 🔥 Start Flask Backend

Run:

```bash
python backend/app.py
```

Backend API will start at:

```
http://localhost:5000
```

---

# 🌐 Start Streamlit Frontend

Open another terminal:

```bash
streamlit run frontend/ui.py
```

Application will open at:

```
http://localhost:8501
```

---

# 🔌 API Documentation

## Health Check

### GET `/health`

Checks whether API is running.

Response:

```json
{
  "status": "API is running"
}
```

---

## Property Price Prediction

### POST `/predict`

Predicts property price based on input features.

### Request:

```json
{
  "area": 2000,
  "rooms": 3
}
```

### Response:

```json
{
  "area": 2000.0,
  "rooms": 3.0,
  "predicted_price": 347820.50,
  "currency": "USD"
}
```

---

## Dataset API

### GET `/dataset`

Returns complete property dataset in JSON format.

---

## Model Information

### GET `/model_info`

Provides:

- Model coefficients
- Evaluation metrics
- Regression details

---

# 📱 Streamlit Application

The frontend contains three main sections:

## 🏠 Property Price Prediction

Users can:

- Enter property area
- Select number of rooms
- Get predicted price instantly
- View prediction results

---

## 📊 Dataset Explorer

Provides:

- Dataset preview
- Scatter plots
- Histograms
- Box plots
- Correlation analysis

---

## 🤖 Model Insights

Displays:

- R² Score
- MAE
- RMSE
- Regression coefficients
- Trendline visualization

---

# 📈 Model Performance

| Metric | Value |
|--------|-------|
| R² Score | ~0.73 |
| MAE | ~$40,000 |
| RMSE | ~$55,000 |

---

# 🧪 Machine Learning Workflow

```
Property Dataset
        |
        ↓
Data Preprocessing
        |
        ↓
Feature Scaling
        |
        ↓
Train-Test Split
        |
        ↓
Linear Regression Training
        |
        ↓
Model Evaluation
        |
        ↓
Save Trained Model
        |
        ↓
Flask API Deployment
        |
        ↓
Streamlit Web Application
```

---

# 🚀 Future Enhancements

- Add more property features:
  - Location
  - Property type
  - Age of property
  - Amenities

- Implement advanced ML models:
  - Random Forest
  - XGBoost
  - Gradient Boosting

- Add user authentication

- Deploy using cloud platforms:
  - AWS
  - Docker
  - Azure
  - Render

---

# 👨‍💻 Author

**Karthikeya Cherukuri**

Integrated M.Tech Software Engineering  
VIT-AP University

GitHub:
https://github.com/VenkataKarthikeya-eng

---

⭐ If you like this project, consider giving it a star!

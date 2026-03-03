# 🎓 Student Exam Performance Predictor

A Machine Learning web application that predicts a student's **Math Score** based on demographic and academic features.

Built using:

- Python
- Flask
- Scikit-learn
- Pandas
- HTML & CSS

---

## 📌 Project Overview

This project predicts a student's **math score** using:

- Gender  
- Race / Ethnicity  
- Parental Level of Education  
- Lunch Type  
- Test Preparation Course  
- Reading Score  
- Writing Score  

The trained ML model is served through a Flask web application.

---

## 📁 Project Structure

```
mlproject/
│
├── app.py                      # Flask application entry point
├── requirements.txt            # Project dependencies
├── README.md                   # Project documentation
│
├── templates/                  # HTML templates
│   └── index.html
|   └── style.css
│
|
│   
│
├── src/                        # Source code
│   │
│   ├── components/             # Training components
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/               # Training & Prediction pipeline
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   │
│   ├── exception.py            # Custom exception handling
│   ├── logger.py               # Logging configuration
│   └── utils.py                # Utility functions
│
├── artifacts/                  # Saved models & preprocessing objects
│   ├── model.pkl
│   └── preprocessor.pkl
│
└── notebook/                   # Jupyter notebooks for experimentation
    └── EDA.ipynb
```

---

## 🚀 Features

✔ Clean web interface for prediction  
✔ Predicts math score using trained regression model  
✔ Proper preprocessing using ColumnTransformer  
✔ Custom exception handling  
✔ Modular ML pipeline structure  
✔ Ready for deployment  

---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/Maaddhhaav21/mlproject.git
cd mlproject
```

---

### 2️⃣ Create Virtual Environment

Mac/Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶ Run the Application

```bash
python app.py
```

Open your browser:

```
http://127.0.0.1:5000/
```

---

## 🧠 How It Works

### 1️⃣ User Input

User provides:

- Gender
- Ethnicity
- Parental Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

---

### 2️⃣ Data Processing

- Form data converted into Pandas DataFrame
- Categorical features encoded
- Numerical features scaled
- Preprocessor loaded from artifacts

---

### 3️⃣ Prediction

- Processed features passed into trained regression model
- Model predicts Math Score
- Result displayed in UI

---

## 📊 Machine Learning Details

- Problem Type: Regression
- Target Variable: Math Score
- Preprocessing:
  - OneHotEncoder
  - StandardScaler
  - ColumnTransformer
- Model: RandomForestRegressor (or selected model)

---

## 🔮 Future Improvements

- Add model evaluation metrics to UI
- Add data visualization
- Add Docker support
- Deploy to cloud (Render / AWS / GCP)
- Add CI/CD pipeline

---

## 👨‍💻 Author

**Madhav Manoj**

---

## 📜 License

MIT License

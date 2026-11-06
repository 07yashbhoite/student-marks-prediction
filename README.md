# Student Exam Score Predictor

A machine learning project that predicts a student's exam score from their daily habits and lifestyle, with an interactive web app built using Streamlit.

## Overview

This project explores how factors like study time, attendance, sleep, and mental health relate to exam performance. It covers the full workflow: data exploration, model training and selection, and deployment as a simple web app.

## Features

- Exploratory data analysis with visualizations
- Training and comparison of multiple regression models
- Best-performing model saved with `joblib`
- Interactive Streamlit app where you adjust inputs with sliders and get a predicted exam score

## Project Structure

```
student-marks-prediction/
├── app.py                          # Streamlit web app
├── notebook.ipynb                  # Data analysis and model training
├── best_model.pkl                  # Trained model
├── student_habits_performance.csv  # Dataset
├── requirements.txt                # Python dependencies
└── README.md
```

## Inputs Used for Prediction

- Study hours per day
- Attendance percentage
- Mental health rating (1-10)
- Sleep hours per night
- [Add any other inputs from your app]

## Tech Stack

- Python
- pandas, NumPy
- scikit-learn
- matplotlib, seaborn
- Streamlit
- joblib

## Getting Started

1. **Clone the repository**
   ```
   git clone https://github.com/YOUR-USERNAME/student-marks-prediction.git
   cd student-marks-prediction
   ```

2. **Install dependencies**
   ```
   python -m pip install -r requirements.txt
   ```

3. **Run the app**
   ```
   python -m streamlit run app.py
   ```

   The app opens in your browser at `http://localhost:8501`.

## Model Performance

| Model | R² Score | MAE |
|-------|----------|-----|
| [Model name] | [value] | [value] |

The best model was saved as `best_model.pkl`.

> Note: the model was trained with scikit-learn version [your version]. Using a different version may cause warnings when loading the model. Check yours with `python -m pip show scikit-learn`.

## Dataset

The dataset (`student_habits_performance.csv`) contains information on student lifestyle habits and exam scores. Source: [https://www.youtube.com/redirect?event=video_description&redir_token=QUlxb01IYXdFUFVOOUlRUzlsOWd5NmVUTV9hdHxBQnJ0NjlrZEx6bGJ4WGpTRmNlZUpGcFRJOXBSSVV6ME53SG8xYzBKQjZMYl9iOHU3dnNMSnVKT3UxWWtrdWtWR205M1pfdHpKakZteFhmLWRhTFViUy1NRnNieDFiOWJ6VDJt&q=https%3A%2F%2Fwww.kaggle.com%2Fdatasets%2Fjayaantanaath%2Fstudent-habits-vs-academic-performance&v=XNGgElLhjD4].

## Future Improvements

- Deploy the app on Streamlit Community Cloud
- Try additional models and hyperparameter tuning
- Add feature importance visualizations

# 🎬 Movie Rating Prediction System

A **Machine Learning project** that predicts movie ratings using IMDb movie-related datasets. The project focuses on data preprocessing, exploratory data analysis, feature engineering, and regression-based machine learning to predict movie ratings and evaluate model performance.

---

## 📌 Project Overview

Movie ratings can be influenced by several factors such as genre, director, actors, number of votes, and movie duration.

This project uses these movie-related features to build a **regression model** capable of predicting movie ratings.

The complete workflow includes:

```text
Dataset
   ↓
Data Cleaning & Preprocessing
   ↓
Exploratory Data Analysis
   ↓
Feature Engineering
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Rating Prediction
   ↓
Model Evaluation
   ↓
Visualization & Insights
```

---

## ✨ Features

* 🧹 Data cleaning and preprocessing
* 📊 Exploratory Data Analysis (EDA)
* ⚙️ Feature engineering using movie metadata
* 🤖 Machine Learning-based movie rating prediction
* 📈 Model performance evaluation
* 📉 Regression metrics analysis
* 📊 Data visualization
* 🔍 Insights from IMDb movie data

---

## 🛠️ Tech Stack

| Technology           | Purpose                              |
| -------------------- | ------------------------------------ |
| **Python**           | Programming language                 |
| **Pandas**           | Data manipulation and preprocessing  |
| **NumPy**            | Numerical operations                 |
| **Matplotlib**       | Data visualization                   |
| **Seaborn**          | Statistical visualization            |
| **Scikit-learn**     | Machine Learning                     |
| **Jupyter Notebook** | Development and analysis environment |

---

## 🤖 Machine Learning Algorithm

### Linear Regression

The project uses **Linear Regression** to predict movie ratings based on the selected movie features.

The model learns relationships between movie attributes and their corresponding ratings using the training dataset.

```text
Movie Features
      ↓
Linear Regression Model
      ↓
Predicted Movie Rating
```

---

## 📊 Regression Evaluation Metrics

The model is evaluated using the following metrics:

### MAE — Mean Absolute Error

Measures the average absolute difference between actual and predicted ratings.

### MSE — Mean Squared Error

Measures the average squared difference between actual and predicted ratings.

### RMSE — Root Mean Squared Error

Provides the square root of the Mean Squared Error and represents prediction error in the same unit as the target variable.

### R² Score

Measures how well the model explains the variation in the target variable.

---

## 📂 Dataset

The project uses **IMDb movie-related datasets** containing information such as:

| Feature      | Description                    |
| ------------ | ------------------------------ |
| `Movie Name` | Name of the movie              |
| `Genre`      | Movie genre                    |
| `Director`   | Movie director                 |
| `Actors`     | Main actors                    |
| `Votes`      | Number of votes                |
| `Duration`   | Movie duration                 |
| `Ratings`    | Movie rating / target variable |

The exact dataset structure may vary depending on the IMDb dataset used.

---

## 🔄 Project Workflow

### 1. Import Dataset

The IMDb dataset is loaded into the Jupyter Notebook using Pandas.

```python
import pandas as pd

df = pd.read_csv("movie_dataset.csv")
```

---

### 2. Data Cleaning & Preprocessing

The dataset is examined and cleaned before applying machine learning.

Key preprocessing steps include:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Cleaning numerical columns
* Processing categorical features
* Preparing the target variable

---

### 3. Exploratory Data Analysis

EDA is performed to understand the dataset and identify meaningful relationships.

The analysis includes:

* Distribution of movie ratings
* Genre analysis
* Vote distribution
* Movie duration analysis
* Relationship between votes and ratings
* Feature correlations

Example visualization:

```text
Movie Features
      │
      ├── Genre
      ├── Duration
      ├── Votes
      ├── Director
      └── Actors
             │
             ▼
       Rating Analysis
```

---

### 4. Feature Engineering

Relevant movie metadata is transformed into features that can be used by the machine learning model.

Feature engineering may include:

* Converting numerical values into usable formats
* Encoding categorical variables
* Extracting useful information from movie metadata
* Selecting relevant prediction features

---

### 5. Train-Test Split

The processed dataset is divided into training and testing sets.

```text
Dataset
   │
   ├───────────────┐
   ▼               ▼
Training Data    Testing Data
   │               │
   ▼               │
Model Training     │
   │               │
   └───────┬───────┘
           ▼
      Evaluation
```

---

### 6. Model Training

The Linear Regression model is trained using the selected movie features.

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

model.fit(X_train, y_train)
```

---

### 7. Prediction

The trained model predicts ratings for the test dataset.

```python
y_pred = model.predict(X_test)
```

---

### 8. Model Evaluation

The predicted ratings are compared with the actual ratings using regression evaluation metrics.

```python
from sklearn.metrics import mean_absolute_error
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
```

The model performance is evaluated using:

```text
MAE
MSE
RMSE
R² Score
```

---

## 📈 Output

The system produces:

* 🎬 Predicted movie ratings
* 📊 Model performance metrics
* 📈 Data visualizations
* 🔍 Insights from movie metadata
* 📉 Comparison between actual and predicted ratings

Example:

```text
Movie: Example Movie
Actual Rating: 7.8
Predicted Rating: 7.5
```

---

## 📁 Project Structure

```text
Movie-Rating-Prediction/
│
├── data/
│   └── movie_dataset.csv
│
├── notebooks/
│   └── movie_rating_prediction.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Movie-Rating-Prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open the Notebook

Open:

```text
movie_rating_prediction.ipynb
```

Run the notebook cells sequentially to perform:

```text
Data Loading
      ↓
Preprocessing
      ↓
EDA
      ↓
Feature Engineering
      ↓
Model Training
      ↓
Prediction
      ↓
Evaluation
```

---

## 📌 Key Concepts Demonstrated

This project demonstrates practical knowledge of:

**Machine Learning • Regression • Data Preprocessing • Exploratory Data Analysis • Feature Engineering • Model Evaluation • Data Visualization • Python • Pandas • Scikit-learn**

---

## 🔮 Future Enhancements

* [ ] Implement additional regression algorithms
* [ ] Compare multiple ML models
* [ ] Perform hyperparameter tuning
* [ ] Improve feature engineering
* [ ] Add cross-validation
* [ ] Build an interactive prediction interface
* [ ] Deploy the model as a web application
* [ ] Add movie recommendation functionality
* [ ] Improve prediction accuracy

---

## 👩‍💻 Author

**Moulika Mallula**

Computer Science & Engineering — Artificial Intelligence & Machine Learning

---

## ⭐ Project Summary

> **A machine learning system that analyzes IMDb movie data and predicts movie ratings using regression techniques.**

```text
IMDb Dataset
     ↓
Data Preprocessing
     ↓
EDA
     ↓
Feature Engineering
     ↓
Linear Regression
     ↓
Rating Prediction
     ↓
MAE | MSE | RMSE | R²
```

---


# 💎 Diamond Price Prediction using Machine Learning

An end-to-end Machine Learning application that predicts the market price of a diamond based on its physical characteristics. The project compares multiple regression algorithms and uses the **Gradient Boosting Regressor** as the final model for prediction. The application is deployed as an interactive **Streamlit** web application.

---

# 📖 Project Overview

Diamond pricing depends on several factors such as carat, cut, color, clarity, depth, table, and physical dimensions. Estimating the price manually is difficult because these features have complex relationships with the target variable.

This project performs complete data preprocessing, exploratory data analysis (EDA), feature engineering, model development, hyperparameter tuning, cross-validation, and deployment. Multiple regression algorithms were evaluated, and the tuned **Gradient Boosting Regressor** was selected as the final model based on its predictive accuracy, low prediction error, and excellent generalization performance.

The application provides a simple web interface where users can enter diamond specifications and instantly receive a predicted price.

---

# 🚀 Features

- Interactive Streamlit web application
- Real-time diamond price prediction
- Gradient Boosting Regressor model
- Complete Machine Learning pipeline
- Data preprocessing and feature engineering
- Hyperparameter tuning using RandomizedSearchCV
- 5-Fold Shuffled Cross Validation
- Feature importance analysis
- Input validation
- Model serialization using Joblib
- Fast predictions using a cached model

---

# 📊 Dataset

The project is trained using the **Diamonds Dataset**, containing information about thousands of diamonds.

## Input Features

| Feature | Description |
|----------|-------------|
| Carat | Weight of the diamond |
| Cut | Diamond cut quality |
| Color | Diamond color grade |
| Clarity | Diamond clarity grade |
| Depth | Total depth percentage |
| Table | Table width percentage |
| x | Length (mm) |
| y | Width (mm) |
| z | Height (mm) |

## Target Variable

- **Price**

---

# ⚙️ Machine Learning Workflow

```
Data Collection
        │
        ▼
Data Cleaning
        │
        ▼
Exploratory Data Analysis (EDA)
        │
        ▼
Feature Engineering
        │
        ▼
Ordinal Encoding
        │
        ▼
Train-Test Split
        │
        ▼
Model Training
        │
        ▼
Hyperparameter Tuning
        │
        ▼
Cross Validation
        │
        ▼
Model Evaluation
        │
        ▼
Pipeline Serialization
        │
        ▼
Streamlit Deployment
```

---

# 🤖 Machine Learning Models

The following regression models were implemented and compared:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- CatBoost Regressor
- AdaBoost Regressor
- LightGBM Regressor

After hyperparameter tuning and model comparison, the **Gradient Boosting Regressor** was selected as the final model due to its superior predictive performance and consistent cross-validation results.

---

# 📈 Model Performance

## Test Dataset

| Metric | Value |
|---------|------:|
| **R² Score** | **0.9824** |
| **MAE** | **272.28** |
| **RMSE** | **525.01** |

## 5-Fold Shuffled Cross Validation

| Metric | Value |
|---------|------:|
| **Mean R² Score** | **0.9831** |
| **Standard Deviation** | **0.00063** |

These results demonstrate that the model achieves high predictive accuracy while maintaining excellent stability and generalization across different data splits.

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- CatBoost
- LightGBM
- Streamlit
- Joblib
- Git
- GitHub

---

# 📂 Project Structure

```
Diamond-Price-Prediction
│
├── app.py
├── diamond_pipeline.pkl
├── Pro1Diamonds.ipynb
├── diamonds.csv
├── requirements.txt
├── README.md
├── Diamond_PPPPT.pptx
└── Diamonds.docx
```

---

# ▶️ Installation

### Clone the repository

```bash
git clone https://github.com/LasyaE/Diamond-Price-Prediction.git
```

### Move into the project directory

```bash
cd Diamond-Price-Prediction
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the application

```bash
streamlit run app.py
```

---

# 💻 Application

Users provide the following inputs:

- Carat
- Cut
- Color
- Clarity
- Depth
- Table
- Length (x)
- Width (y)
- Height (z)

The application preprocesses the user inputs using the saved encoder and predicts the diamond price using the trained **Gradient Boosting Regressor**.

---

# 📌 Future Enhancements

- Batch prediction using CSV upload
- Live exchange rate conversion
- Docker containerization
- CI/CD deployment
- Model monitoring
- Prediction history dashboard

---

# 🚀 Live Demo



---

# 👩‍💻 Author

**Lasya Reddy**

B.Tech in Computer Science Engineering (Artificial Intelligence & Machine Learning)

GitHub: https://github.com/LasyaE

---

# ⭐ Acknowledgement

This project was developed as an end-to-end Machine Learning application to demonstrate practical skills in data preprocessing, exploratory data analysis, feature engineering, model development, evaluation, hyperparameter tuning, deployment, and web application development using Python and Streamlit.

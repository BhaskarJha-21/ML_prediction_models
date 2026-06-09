# Machine Learning Prediction Model for Antenna Optimization 📡🤖

This project applies Machine Learning techniques to predict antenna **S11** values using antenna design parameters. A Random Forest Regression model is trained on simulation data to estimate antenna performance for new configurations, reducing the need for repeated simulations.

---

## 📌 Project Overview

The objective of this project is to predict antenna performance metrics using supervised machine learning.

The model learns the relationship between antenna design parameters and the corresponding S11 values, helping accelerate antenna design optimization and analysis.

---

## 🚀 Features

- Data preprocessing and feature scaling
- Random Forest Regression model
- Model performance evaluation
- Prediction on unseen antenna configurations
- Visualization of actual vs predicted values
- Automated prediction generation

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📂 Repository Structure

```text
ML_prediction_models/
│
├── README.md
│
├── notebook/
│   └── Training_model.ipynb
│
└── data/
    ├── training_data.csv
    ├── testing_data.csv
    └── prediction_data.csv
```

---

## 📊 Dataset Features

The model uses the following antenna design parameters:

| Feature |
|----------|
| Frequency |
| Ws |
| H1 |
| D1 |
| Lp |
| W1 |

### Target Variable

```text
S11
```

---

## ⚙️ Machine Learning Pipeline

### 1. Data Loading

Training, testing, and prediction datasets are loaded using Pandas.

### 2. Data Preprocessing

- Feature extraction
- Feature scaling using StandardScaler

### 3. Model Training

A Random Forest Regressor is trained using:

```python
RandomForestRegressor(
    n_estimators=100,
    random_state=42
)
```

### 4. Model Evaluation

The model is evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### 5. Prediction Generation

Predictions are generated for unseen antenna configurations directly within the notebook.

### 6. Visualization

The notebook generates an Actual vs Predicted regression plot to evaluate model performance.

---

## 📈 Results

The notebook displays:

- Model evaluation metrics
- Prediction results
- Actual vs Predicted visualization
- Generated S11 predictions for new antenna configurations

All outputs are produced directly inside:

```text
notebook/Training_model.ipynb
```

---

## ▶️ Running the Project

Clone the repository:

```bash
git clone https://github.com/BhaskarJha-21/ML_prediction_models.git
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebook/Training_model.ipynb
```

and run all cells.

---

## 🎯 Applications

- Antenna Design Optimization
- RF Engineering
- Wireless Communication Systems
- Design Space Exploration
- Simulation Time Reduction

---

## 👨‍💻 Author

Bhaskar Kumar Jha
B.Tech Electronics & Communication Engineering
National Institute of Technology Delhi

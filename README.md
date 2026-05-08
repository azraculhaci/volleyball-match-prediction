# Volleyball Match Outcome Prediction using Machine Learning

A machine learning project focused on predicting volleyball match outcomes using team performance statistics and classification algorithms.

---

## Project Overview

This project analyzes volleyball team statistics and builds predictive machine learning models to estimate match outcomes.

The workflow includes:

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Model training
- Cross-validation
- Performance evaluation
- Feature importance analysis

The main objective is to determine which volleyball performance metrics contribute most to winning matches.

---

## Dataset

The dataset contains volleyball team statistics such as:

- Aces per set
- Assists per set
- Team attacks per set
- Blocks per set
- Digs per set
- Hitting percentage
- Kills per set
- Opponent hitting percentage

A binary target variable was created based on win/loss percentage:

- `1` → Winning team
- `0` → Losing team

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

---

## Machine Learning Models

The following classification algorithms were implemented and compared:

- Random Forest Classifier
- Logistic Regression
- Gradient Boosting Classifier

Cross-validation was used to evaluate model stability and generalization performance.

---

## Data Preprocessing

The preprocessing pipeline includes:

- Missing value handling using `SimpleImputer`
- Feature scaling using `StandardScaler`
- Stratified train-test split
- Data leakage prevention

### Data Leakage Prevention

The following columns were excluded from training because they directly reveal match outcomes:

- `W`
- `L`
- `win_loss_pctg`

---

## Exploratory Data Analysis (EDA)

Several visualizations were created to better understand the dataset:

- Feature distributions
- Correlation heatmaps
- Scatter plots
- Target class distribution
- Confusion matrix
- Feature importance charts

---

## Model Evaluation Metrics

The models were evaluated using:

- Accuracy Score
- Cross-Validation Accuracy
- Confusion Matrix
- Classification Report
- Baseline Comparison

---

## Feature Importance

The project analyzes which statistics most strongly affect volleyball match success.

Key performance indicators include:

- Kills per set
- Hitting percentage
- Blocks per set
- Opponent hitting percentage

---

## Project Structure

```text
├── volleyball_match_prediction.ipynb
├── volleyball_matches.csv
├── volleyball_model.pkl
└── README.md
```

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/volleyball-match-prediction.git
```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

### 3. Run the Notebook

Open:

```text
volleyball_match_prediction.ipynb
```

using Jupyter Notebook or VS Code.

---

## Results

The machine learning models achieved strong classification performance in predicting volleyball match outcomes.

Among the tested models, Random Forest produced the best overall performance.

---

## Future Improvements

Possible future enhancements include:

- Hyperparameter optimization
- Deep learning models
- Real-time match prediction
- Larger datasets
- Advanced feature engineering
- Web deployment using Flask or FastAPI

---

## Author
Developed by Azra Culhacı

# Titanic Survival Prediction & Dataset Optimization 🚢

Visualized exploratory data analysis (EDA), automated memory optimization, and a Random Forest Machine Learning pipeline built with Python and Pandas on the classic Titanic dataset.

---

## Key Highlights

- **Memory Optimization**: Reduced dataset size in memory from **278.87 MB** down to **127.80 KB** (a **~54.17%** memory save) by optimizing data types (`int8` and `category`).
- **Data Cleaning & Handling**: Imputed missing values for `age` (median) and `embarked` (mode).
- **Feature Engineering**: Engineered new features such as `family_size`, `alone`, and numerical `male` indicators.
- **Predictive Modeling**: Trained a `RandomForestClassifier` baseline model achieving **80.45%** survival prediction accuracy.
- **Visual Exploratory Analysis**: Integrated Seaborn and Matplotlib for feature distributions and demographic survival trends.

---

## Project Workflow

1. **Dataset Loading & Downcasting**  
   Converts numerical and categorical columns to low-footprint datatypes (`int8`, `category`).
2. **Missing Value Imputation**  
   Fills missing entries systematically without introducing lookahead bias.
3. **Feature Construction**  
   Creates relational indicators (`family_size`, `alone`) to boost tree-based model performance.
4. **Machine Learning Baseline**  
   Splits data $80/20$ for training/testing and evaluates model accuracy using Scikit-Learn.
5. **Data Visualization**  
   Generates demographic survival plots and feature relationships.

---

## Tech Stack & Dependencies

- **Language**: Python 3.x
- **Data Manipulation**: `pandas`, `numpy`
- **Visualization**: `seaborn`, `matplotlib`
- **Machine Learning**: `scikit-learn`

---

## Model Evaluation

| Model | Test Accuracy | Features Used |
| :--- | :---: | :--- |
| **Random Forest Baseline** | **80.45%** | `pclass`, `age`, `fare`, `family_size`, `alone`, `male` |

---

## Quick Start & Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Mahmoud4265/Real-World-Data-Pipeline-Memory-Optimization-Engine.git
   cd Real-World-Data-Pipeline-Memory-Optimization-Engine
   ```
2.**Install required packages**:

```Bash
pip install pandas numpy matplotlib seaborn scikit-learn
```


3-**Run the analysis notebook**:
Launch Jupyter Notebook or VS Code and execute notebook.ipynb.

# ML Placement Predictor

A beginner-friendly toy machine learning project that predicts whether a student will be placed based on their **CGPA** and **IQ**. This project is designed for educational purposes and demonstrates a basic ML workflow using Python and scikit-learn.

---

## Features

- Binary classification using Logistic Regression  
- Two input features: `CGPA` and `IQ`  
- Data visualization and decision boundary plotting  
- Saves the trained model using `pickle`

---

## What You’ll Learn

- How to load and preprocess data  
- How to split data into training and test sets  
- How to scale features using `StandardScaler`  
- How to train a logistic regression model  
- How to evaluate model accuracy  
- How to visualize decision boundaries  
- How to save and reuse a trained model

---

## Project Structure

```text
placement-predictor/
├── toy_project.ipynb       # Jupyter notebook with full code
├── placement.csv           # Dataset file (should be added separately)
├── model.pkl               # Saved machine learning model
├── requirements.txt        # Python package dependencies
└── README.md               # Project documentation (this file)
```

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Shivansh1205/toy-project
cd toy-project
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

Open `toy_project.ipynb` in Jupyter Notebook or Google Colab, and run all the cells step by step to:

- Load the data  
- Train the model  
- Evaluate performance  
- Visualize results

---

## Dataset Format

The dataset should be named `placement.csv` and contain the following columns:

| cgpa | iq  | placement |
|------|-----|-----------|
| 8.5  | 120 | 1         |
| 6.7  | 100 | 0         |

- `cgpa`: Student's CGPA  
- `iq`: Student's IQ score  
- `placement`: `1` if placed, `0` if not placed

---

## Visualization

- Scatter plot showing CGPA vs IQ, color-coded by placement  
- Decision boundary plot using `mlxtend.plot_decision_regions` to visualize model classification zones

---

## Example Prediction

```python
Input: CGPA = 8.5, IQ = 130  
Output: Placed
```

---

## Requirements

```
numpy
pandas
matplotlib.pyplot
sklearn.model_selection
sklearn.preprocessing
sklearn.linear_model
sklearn.metrics
mlxtend.plotting
pickle
```

Install them using:

```bash
pip install -r requirements.txt
```

To generate `requirements.txt` yourself:

```bash
pip freeze > requirements.txt
```

---

## Disclaimer

This is a toy ML project for educational purposes only. The model is trained on a small, synthetic dataset and is not intended for use in real-world placement scenarios.

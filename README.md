# ANN vs Decision Tree: Cooling Load Prediction

Week 3 Assignment — Soft Computing Course  
Institut Teknologi Sepuluh Nopember (ITS)

## Overview

This project compares two machine learning approaches for predicting the **Cooling Load** of residential buildings using the [Energy Efficiency dataset](https://archive.ics.uci.edu/dataset/242/energy+efficiency) from the UCI Machine Learning Repository.

| Approach | Model |
|---|---|
| Neural Network | Multi-Layer Perceptron (MLP) via Keras/TensorFlow |
| Baseline | Decision Tree Regressor via scikit-learn |

Both models are evaluated on **MSE**, **MAE**, **R2 Score**, and **runtime**.

## Dataset

- **Source**: UCI Machine Learning Repository — Energy Efficiency Data Set
- **File**: `ENB2012_data.xlsx`
- **Samples**: 768
- **Input features (X1–X8)**: Relative Compactness, Surface Area, Wall Area, Roof Area, Overall Height, Orientation, Glazing Area, Glazing Area Distribution
- **Target (Y2)**: Cooling Load

## Project Structure

```
sc-ann-assignment/
├── notebook.ipynb       # Main notebook (all sections)
├── ENB2012_data.xlsx    # Dataset file (place in same folder as notebook)
├── requirements.txt     # Python dependencies
└── README.md
```

## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/adhiraga/sc-ann-assignment.git
cd sc-ann-assignment
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

Or run Section 0 inside the notebook directly.

### 3. Place the dataset
Make sure `ENB2012_data.xlsx` is in the same folder as `notebook.ipynb`.

### 4. Run the notebook
Open `notebook.ipynb` in VS Code or Jupyter and run cells from top to bottom.

## Notebook Sections

| Section | Description |
|---|---|
| 0 | Install dependencies |
| 1 | Import libraries |
| 2 | Load and explore dataset |
| 3 | Separate features and target |
| 4 | Train-test split and feature scaling |
| 5 | Decision Tree Regressor (baseline) |
| 6 | Neural Network MLP (Keras) |
| 7 | Model comparison table |
| 8 | Analysis and interpretation |

## Dependencies

See `requirements.txt`. Main libraries:
- `pandas`, `numpy`
- `scikit-learn`
- `tensorflow`
- `openpyxl`

# Stock Market Prediction Using Machine Learning

This project predicts stock market trends using machine learning models. It includes historical stock data, trained models, and a Flask web application to visualize predictions.

---

## Project Structure

```
├─ __pycache__/                 # Python cache files
├─ individual_stocks_5yr/       # Historical stock data
├─ model/                       # Machine learning models and preprocessing
├─ static/                      # Static files (CSS, JS)
├─ templates/                   # HTML templates for Flask app
├─ app.py                       # Flask application
├─ poly.pkl                      # Pre-trained polynomial transformer
├─ regressor.pkl                 # Pre-trained regression model
├─ requirements.txt             # Python dependencies
├─ runtime.txt                  # Python version for Render deployment
├─ train_models.py              # Script to train models
├─ upload.csv                   # Sample stock data
├─ utils.py                     # Utility functions
└─ README.md                    # Project documentation
```

---

## Features

* Predicts stock trends using historical stock data
* Machine learning models trained on 5 years of stock data
* Flask web application for user interaction
* Easy deployment on [Render](https://render.com/) using `runtime.txt` and pinned dependencies

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/PavanReddy2924/stock-market-pred.git
cd stock-market-pred
```

2. Create a virtual environment and activate it:

```bash
python3 -m venv venv
source venv/bin/activate       # Linux/macOS
venv\Scripts\activate        # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Notes

* Make sure your `requirements.txt` lists packages compatible with Python 3.8.
* The trained models (`poly.pkl` and `regressor.pkl`) are included, so no retraining is required to run the app.
* Static files and templates are in `static/` and `templates/` folders respectively.

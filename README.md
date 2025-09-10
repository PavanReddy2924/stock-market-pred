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
├─ poly.pkl                     # Pre-trained polynomial transformer
├─ regressor.pkl                # Pre-trained regression model
├─ requirements.txt             # Python dependencies
├─ runtime.txt                  # Python version (optional, for deployment)
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
* Ready for deployment on platforms like Render or Heroku

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

## Usage

1. Run the Flask app locally:

```bash
python app.py
```

2. Open your browser and go to:

```
http://127.0.0.1:5000
```

3. Upload CSV files of stock data or use the sample `upload.csv` to predict trends.

---

## Deployment

For deployment on services like Render or Heroku:

1. Ensure `runtime.txt` specifies the Python version if required (e.g., `python-3.8.16`).
2. Set the start command according to the platform, for example:

```bash
gunicorn app:app --bind 0.0.0.0:$PORT
```

3. Push the repository to GitHub and connect it to your deployment platform.

---

## Notes

* The trained models (`poly.pkl` and `regressor.pkl`) are included.
* Static files and templates are located in `static/` and `templates/` folders respectively.
* `requirements.txt` contains all necessary dependencies for running the project.

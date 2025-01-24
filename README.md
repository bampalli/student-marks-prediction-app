# Student Mark Predictor

This project is a Flask-based web application that predicts student marks based on study hours using a trained machine learning model.

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Endpoints](#endpoints)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)

## Overview
This application allows users to input study hours and predict the expected marks based on a pre-trained machine learning model. The predictions are logged and saved in a CSV file for future analysis.

## Project Structure
```
Student-Mark-Predictor/
│-- static/                # Static files (CSS, images, etc.)
│-- templates/             # HTML templates
│   └── index.html          # Main UI page
│-- Desktop.pkl            # Pre-trained model file
│-- app.py                  # Flask application
│-- smp_data_from_app.csv   # CSV file to store predictions
│-- requirements.txt        # Dependencies
│-- README.md               # Project documentation
```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/student-mark-predictor.git
   cd student-mark-predictor
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Ensure the model file `Desktop.pkl` is placed in the project directory.

## Usage

1. Run the Flask app:
   ```bash
   python app.py
   ```

2. Open your browser and go to:
   ```
   http://127.0.0.1:5000
   ```

3. Enter the study hours and click **Predict Marks** to get the predicted results.

## Model Details
- The model used for prediction is pre-trained and loaded from the `Desktop.pkl` file.
- It accepts the number of study hours as input and predicts marks as output.
- The predictions are logged into `smp_data_from_app.csv`.

## Endpoints

| Route      | Method | Description                              |
|------------|--------|------------------------------------------|
| `/`        | GET    | Renders the home page                    |
| `/predict` | POST   | Processes input and returns predictions  |

## Technologies Used
- **Programming Language:** Python
- **Framework:** Flask
- **Libraries:** Pandas, NumPy, Joblib
- **Frontend:** HTML, CSS

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push to your fork and submit a pull request.

---


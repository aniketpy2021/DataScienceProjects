# Wine Quality Prediction Project

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-2.x-green.svg)](https://flask.palletsprojects.com/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-%23FF69B4.svg?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

## Introduction

This project is a Python-based application that predicts the quality of wine based on various chemical features. It utilizes a machine learning model trained on a provided dataset and deploys the model as a web application using Flask, allowing users to input wine characteristics and receive a quality prediction.

## Objective

The primary purpose of this project is to predict the quality of wine using a Multiple Linear Regression model trained on a dataset provided in CSV format. The results of the prediction are then rendered through a user-friendly web interface built with Flask.

## Problem Statement

Given a dataset containing various independent variables representing the chemical composition of wine (e.g., acidity, sugar content, alcohol level), the goal is to build a predictive model. For testing and demonstration purposes, we focus on understanding the relationship between these wine content variables and the dependent variable, **Quality**, to predict the quality score of a given wine sample.

## Dataset Information

The project utilizes a training dataset stored in a CSV file named `"Wine Quality Dataset.csv"`. This dataset contains multiple independent variables representing the chemical properties of wine, and a dependent variable, `Quality`, which is the target variable we aim to predict. The dataset provides the necessary information to train the machine learning model.

## Model Development

### Algorithms Used

* **Multiple Linear Regression:** This project employs a Multiple Linear Regression algorithm to model the linear relationship between the independent wine content variables and the dependent `Quality` variable. The model is trained on the provided dataset to learn these relationships.

### Model Persistence

The trained Multiple Linear Regression model is saved to a file named `linear.pkl` using a Python serialization library (like `pickle`). This allows for the model to be loaded and used for predictions without retraining every time the application runs.

## Model Deployment

### Deployment Method

The trained machine learning model is deployed as a web API using the Flask framework. This allows users to interact with the model through a web browser. The `app.py` script contains the Flask application logic, which handles user input from a web form, loads the pre-trained model, makes predictions, and displays the results on a web page. The web page is rendered using the `index.html` template located in the `templates` directory.

## Steps to Run the Deployed Model

Follow these steps to run the wine quality prediction web application locally:

1.  **Prerequisites:** Ensure you have Python 3.x and pip installed on your system.

* **Python 3.x:** Make sure you have Python 3 installed. You can download it from [https://www.python.org/downloads/](https://www.python.org/downloads/).
* **Git:** Git is required to clone the repository. You can download it from [https://git-scm.com/downloads](https://git-scm.com/downloads).
* **pip:** pip is the package installer for Python and usually comes bundled with Python installations.

2.  **Clone the Repository:**
    Open your terminal or command prompt and run:

    ```bash
    git clone [https://github.com/](https://github.com/)<your_github_username>/DataScienceProjects.git
    ```
    (Replace `<your_github_username>` with the actual username of the repository owner).

3.  **Navigate to the Project Directory:**

    ```bash
    cd DataScienceProjects/WineQuality
    ```

4.  **Create and Activate a Virtual Environment (Recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On macOS and Linux
    venv\Scripts\activate   # On Windows
    ```

5.  **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

6.  **Run the Flask Application:**

    ```bash
    python app.py
    ```

7.  **Access the Application in Your Browser:**
    Open your web browser and go to the address provided in the terminal output (usually `http://127.0.0.1:5000/`).

8.  **Interact with the Application:**
    You should see a web page with input fields for the wine content variables. Enter the values for the desired wine sample and click the "Predict Quality" button. The predicted wine quality will be displayed on the page.

## Contributing

Aniket Patankar

## License

Created for Learning Purpose

# Laptop Price Prediction

This project predicts laptop prices based on various features using a Machine Learning model. The model is trained using Jupyter Notebook and deployed using a Flask web application.

## Table of Contents
- [Overview](#overview)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Project Structure](#project-structure)
- [License](#license)

## Overview
The goal of this project is to predict the price of a laptop based on its specifications. The model is built using machine learning techniques in Jupyter Notebook and exported as a pickle (`.pkl`) file. A Flask web application is used to serve predictions.

## Technologies Used
- Python
- Jupyter Notebook
- Flask
- Scikit-Learn
- Pandas
- NumPy
- Pickle

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/KADTLAKSHAN/laptop-price-prediction.git
   cd laptop-price-prediction
   ```

2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

4. Run the Flask app:
   ```sh
   python app.py
   ```

## Usage
Once the Flask app is running, you can access it at `http://127.0.0.1:5000/` and use API endpoints to get predictions.

## API Endpoints

- `POST /predict`: Sends laptop specifications as JSON input and receives a predicted price.

  Example request:
  ```json
  {
      "brand": "Dell",
      "ram": 16,
      "processor": "Intel Core i7",
      "storage": 512
  }
  ```

  Example response:
  ```json
  {
      "predicted_price": 1200
  }
  ```

## Project Structure
```
├── model building.ipynb   # Jupyter Notebook for training the model
├── app.py                 # Flask web application
├── model.pkl              # Trained ML model
├── requirements.txt       # Dependencies
├── README.md              # Project documentation
```

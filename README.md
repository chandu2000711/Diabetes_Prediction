
# Diabetes Prediction API

This project provides a FastAPI-based web service for predicting the likelihood of diabetes based on various medical parameters. The API is designed to be simple and easy to use, accepting input data in JSON format and returning predictions as JSON.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

## Overview

This project uses a machine learning model to predict the likelihood of a person having diabetes. The model is served using FastAPI, a modern, fast (high-performance), web framework for building APIs with Python 3.7+ based on standard Python type hints.

## Features

- Predict diabetes likelihood using various medical features.
- Fast and efficient API built with FastAPI.
- Deployed on a free platform for easy access.

## Getting Started

Follow the instructions below to set up and run the project locally.

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/diabetes-prediction-api.git
    cd diabetes-prediction-api
    ```

2. **Create and activate a virtual environment**:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. **Run the FastAPI application**:
    ```bash
    uvicorn main:app --reload
    ```

2. **Access the API**:
   Open your web browser and go to `http://127.0.0.1:8000/docs` to view the automatically generated Swagger documentation.

### API Endpoints

- `POST /predict`: Accepts input data in JSON format and returns the predicted likelihood of diabetes.

Example request:
```json
{
    "Pregnancies": 6,
    "Glucose": 148,
    "BloodPressure": 72,
    "SkinThickness": 35,
    "Insulin": 0,
    "BMI": 33.6,
    "DiabetesPedigreeFunction": 0.627,
    "Age": 50
}


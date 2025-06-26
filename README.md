# House-Price-Prediction-Web-application-Deployment-on-Heroku

# House Price Prediction – Heroku-Deployed Flask Web App

A machine learning web application built with **Flask** to predict house prices using a **Linear Regression** model. The app was containerised in a virtual environment and deployed to **Heroku** via the CLI. For details on model development and local Flask deployment, see the companion repository: [ML-Based-House-Price-Prediction-Web-App](https://github.com/UdonnaM/ML-Based-House-Price-Prediction-Web-App)


---

## Table of Contents

* [Overview](#overview)
* [Features](#features)
* [Tech Stack](#tech-stack)
* [Project Structure](#project-structure)
* [Getting Started](#getting-started)
* [Model Deployment (Heroku)](#model-deployment-heroku)
* [Screenshot of Deployed Web Application](#Screenshot-of-Deployed-Web-Application)
* [Project Summary](#Project-Summary)

---

## Overview

This project demonstrates how a simple machine learning model for house price prediction can be deployed as a live web app using Flask and hosted on Heroku. The model was trained using `scikit-learn`, wrapped in a Python Flask server, and served via HTML templates.

---

## Features

* Clean UI for inputting house-related features
* Predicts house prices in real-time using a trained Linear Regression model
* Virtual environment setup for dependency isolation
* Hosted on Heroku with public accessibility

---

## Tech Stack

| Tool         | Usage                          |
| ------------ | ------------------------------ |
| Python       | Core programming language      |
| Flask        | Web framework                  |
| scikit-learn | Machine Learning               |
| HTML/CSS     | Frontend interface             |
| Heroku       | App hosting and deployment     |
| Git & CLI    | Version control and deployment |
| Virtualenv   | Environment management         |

---

## Project Structure

```bash
houseprice_app/
│
├── templates/
│   └── index.html               # Frontend template
│
├── static/                      # (Optional) CSS or JS
│
├── model.pkl                    # Serialized trained model
├── app.py                       # Main Flask application
├── requirements.txt             # Python dependencies
├── Procfile                     # Heroku process file
├── runtime.txt                  # Python version on Heroku
├── start_app.bat                # Windows shortcut to run app
└── README.md                    # This file
```

---

## Getting Started (Local Setup)

```bash
# 1. Clone repo and move into project directory
git clone https://github.com/your-username/House-Price-Prediction-Web-application-Deployment-on-Heroku.git
cd House-Price-Prediction-Web-application-Deployment-on-Heroku

# 2. Set up virtual environment
python -m venv venv
venv\Scripts\activate  # On Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the app
python app.py
```

Visit `http://127.0.0.1:5000` in your browser.

---

##  Model Deployment (Heroku)

### Prerequisites

* [x] Install Heroku CLI
* [x] Login via `heroku login`
* [x] Create Heroku app: `heroku create udonnas-houseprice-app`
* [x] Add and commit project with Git

### Deployment Steps

```bash
# Initialize Git and commit files
git init
git add .
git commit -m "Initial commit"

# Create Heroku app
heroku create udonnas-houseprice-app

# Push to Heroku
git push heroku master

# Open app in browser
heroku open
```

🔗 Deployed App: [https://udonnas-houseprice-app.herokuapp.com](https://udonnas-houseprice-app-c44eaa628f09.herokuapp.com/)

---

## Screenshot of Deployed Web Application

The image below displays the user interface of the Flask-based web form and the predicted house price result after successful deployment on Heroku.

![House Price Prediction Screenshot](screenshots/Web%20app%20image.jpg)

---

## Project Summary

This project demonstrates the complete cycle of building, containerising, and deploying a machine learning web application using Flask and Linear Regression. It highlights key skills such as model integration into a web framework, virtual environment management, and cloud deployment via the Heroku CLI. While the primary goal was deployment, this project also reflects best practices in organising machine learning pipelines for real-world use.

The successful deployment marks the culmination of local development efforts and showcases practical knowledge in full-stack machine learning workflows.

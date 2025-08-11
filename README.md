Linear Regression Taxi Fare Prediction
This project is part of Google’s Machine Learning Crash Course (MLCC) exercises.
It demonstrates how to build, train, and evaluate a linear regression model to predict taxi fares in Chicago using historical trip data.

📌 Project Overview
The goal is to:

Load and explore the Chicago Taxi Trips dataset.

Identify correlations between trip features and fare amount.

Build a simple linear regression model with Keras.

Experiment with different features and hyperparameters.

Evaluate model performance using RMSE and loss curves.

📊 Dataset
Source: City of Chicago Taxi Trips

Subset: Two-day period in May 2022

Key features:

TRIP_MILES — Distance of the trip

TRIP_SECONDS — Duration of the trip

TRIP_MINUTES — Derived from TRIP_SECONDS

FARE — Fare amount (label)

COMPANY — Taxi company

PAYMENT_TYPE — Payment method

TIP_RATE — Tip percentage

🛠 Installation
Install dependencies:

bash
Copy
Edit
pip install google-ml-edu==0.1.3 keras~=3.8.0 matplotlib~=3.10.0 numpy~=2.0.0 pandas~=2.2.0 tensorflow~=2.18.0
🚀 Usage
Run the notebook in Google Colab or locally:

bash
Copy
Edit
jupyter notebook linear_regression_taxi.ipynb
Main steps in the notebook:

Load dataset

Explore dataset (summary stats, correlations, visualizations)

Train model with:

Single feature (TRIP_MILES)

Hyperparameter tuning

Two features (TRIP_MILES + TRIP_MINUTES)

Evaluate results using RMSE and plots.

📈 Results
Best RMSE (two features): ~3.48

Strongest correlation to fare: TRIP_MILES

Weakest correlation to fare: TIP_RATE

Using two features improved prediction accuracy compared to a single feature.


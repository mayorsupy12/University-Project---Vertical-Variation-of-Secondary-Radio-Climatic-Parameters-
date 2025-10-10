# Vertical Analysis of Selected Secondary Radio-Climatic Parameters Using UAVs-
### This is my final year university project at the Federal University of Technology Akure in fulfillment of the requirement for the award of Bachelor of Technology (B.Tech) Degree in Physics Electronics.

### Project Overview

This project investigates the vertical variation of key secondary radio-climatic parameters that influence the propagation of electromagnetic waves. primary radio climatic Data (Temperature, Pressure, Relative Humidity) was collected over 30 days at four altitudes:
0 m, 25 m, 50 m, and 75 m, across six synoptic hours daily (6am, 9am, 12pm, 3pm, 6pm, 9pm).

#### The parameters analyzed include:

Radio Refractivity (N)

Refractivity Gradient (dN/dh)

Geo-Climatic Factor (ΔN)


A UAV (drone) equipped with meteorological sensors was used to capture high-resolution atmospheric data. This approach allows better insight into boundary-layer behavior compared to conventional radiosonde or ground-only observations.

#### The study provides a detailed analysis of:

Diurnal and daily variations

Vertical structure of refractivity

Implications for terrestrial radio communication systems

Potential for ducting, super-refraction, and signal fading

### Data Collection & Processing

UAV mounted with temperature, pressure, and humidity sensors

Measurements taken at fixed altitudes

Data preprocessed using Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)

Refractivity computed using modified Smith–Weintraub equations

Gradient and geo-climatic parameters derived using atmospheric formulas

### Visualizations Included

#### The analysis features visual plots such as:

Vertical profiles of refractivity

Layer-by-layer refractivity gradients

Diurnal variation across altitudes

Combined surface vs elevated gradients

These plots were used to interpret atmospheric effects on radio-wave propagation.

### Machine Learning Model

A Decision Tree Regressor was trained to predict radio refractivity based on environmental inputs:

Humidity

Temperature

Pressure

The trained model was exported in both:

regressor_model.joblib

regressor_model.onnx formats

This enables integration into applications for radio link planning, propagation effect prediction, and real-time atmospheric monitoring.

### Model Purpose

The model helps determine refractivity levels to infer likely radio propagation conditions such as:

Ducting

Super-refraction

Standard propagation

Sub-refraction

Anomalous conditions

### Deployment

#### A Gradio-based interface and deployment script was prepared to host this model on Hugging Face Spaces, allowing user interaction via a browser.
#### https://huggingface.co/spaces/mayorsupy/Radio-Refractivity_Predictor

📂 Repository Contents (Suggested Structure)
├── dataset/
├── jupyter_notebooks.ipyn/
├── models/
│   ├── regressor_model.joblib
│   ├── regressor_model.onnx
├── plots/
├── deploy_to_hf.py
├── app.py or gradio_app.py
└── README.md

### Summary

This project offers a practical UAV-based approach to understanding the vertical structure of atmospheric refractivity and its influence on radio communication.
Through data analysis and machine learning, it provides scientifically grounded insights that can improve network planning, radar performance, microwave link reliability, and spectrum management.

# green-ops-hackathon
Wind turbine scada data for early fault detection

Dataset used - https://www.kaggle.com/datasets/azizkasimov/wind-turbine-scada-data-for-early-fault-detection

Predictive Maintenance for Renewable Energy Assets

Overview

This project focuses on developing an AI-powered predictive maintenance system for renewable energy assets like wind turbines and solar panels. Using SCADA data and deep learning techniques, the system detects early signs of equipment degradation, allowing proactive maintenance to reduce downtime and improve energy efficiency.

Features

SCADA-Based Anomaly Detection: Extracts key metrics such as power output, rotor speed, and environmental conditions.

Deep Learning for Anomaly Detection: Uses autoencoders and time-series models (RNNs/Transformers) to predict failures.

Multi-Sensor Data Fusion: Combines sensor readings to improve failure detection accuracy.

Failure Prediction Modeling: Estimates the Remaining Useful Life (RUL) of components for proactive scheduling.

Setup Instructions

Install Required Libraries:

pip install kaggle numpy pandas tensorflow scikit-learn matplotlib seaborn

Upload Kaggle API Key:

Upload the kaggle.json file.

Move it to the appropriate directory:

from google.colab import files
files.upload()  # Upload the kaggle.json file

Set permissions and configure the environment:

mkdir -p ~/.kaggle
mv kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json

Download Dataset:

kaggle datasets download -d <dataset-name>
unzip <dataset-name>.zip

Run the Jupyter Notebook:

Open the notebook (wind_turbin.ipynb) and execute the cells to preprocess data, train models, and visualize results.

Usage Instructions

Preprocessing: The notebook cleans and processes SCADA logs, handling missing values and outliers.

Model Training: The deep learning model is trained to detect anomalies and predict failures.

Visualization: Graphs and charts illustrate performance trends and failure predictions.

Authors
Team Byte 
( Aastha Shinde , Varad Dongarkar ) 

Future Improvements

Improve model generalization for different asset types.

Deploy in a real-time monitoring system for live anomaly detection.

Optimize model efficiency for lower latency predictions.

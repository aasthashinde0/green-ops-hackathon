# Predictive Maintenance for Renewable Energy Assets

## 📌 Overview
This project aims to implement a **Predictive Maintenance system for Renewable Energy Assets using Autoencoders**  for anomaly detection and Recurrent Neural Networks (RNNs) for time-series forecasting. The goal is to predict equipment failures and maintenance needs before they occur, improving efficiency and reducing downtime.

### 📂 Dataset
- **Source**: [Kaggle - Wind Turbine SCADA Data for Early Fault Detection](https://www.kaggle.com/datasets/azizkasimov/wind-turbine-scada-data-for-early-fault-detection)

---
Methodology

1. Anomaly Detection using Autoencoders
- Trained an Autoencoder on normal operational data.
- Used Reconstruction Loss to detect anomalies.
- Set a threshold to classify faulty conditions.

2. Time-Series Forecasting using RNN
- Implemented a Recurrent Neural Network (RNN) to forecast future values.
- Used historical data to train the model.
- Compared predicted values with actual values to assess model performance.

---
## 🛠 Setup Instructions
### 1️. Install Required Libraries:
```bash
pip install kaggle numpy pandas tensorflow scikit-learn matplotlib seaborn
```

### 2️. Upload Kaggle API Key:
Upload your `kaggle.json` file.
```python
from google.colab import files
files.upload()  # Upload the kaggle.json file
```

### 3️. Configure Kaggle Credentials:
```bash
mkdir -p ~/.kaggle
mv kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```

### 4️. Download and Extract Dataset:
```bash
kaggle datasets download -d azizkasimov/wind-turbine-scada-data-for-early-fault-detection
unzip wind-turbine-scada-data-for-early-fault-detection.zip
```

### 5️⃣ Run the Jupyter Notebook:
- Open `wind_turbine.ipynb`
- Execute the cells to **preprocess data, train models, and visualize results**.

---
## 📝 Usage Instructions
### 🔹 **Preprocessing**
- Cleans and processes **SCADA logs**
- Handles **missing values and outliers**

### 🔹 **Model Training**
- Trains a **deep learning model** for anomaly detection and failure prediction

### 🔹 **Visualization**
- **Graphs and charts** illustrate performance trends and failure predictions

---
## 🔮 Future Improvements
- Fine-tune RNN model with **more training data**.
- Experiment with LSTMs/GRUs for improved forecasting
- Deploy the model as a real-time predictive maintenance tool.

---
## 👥 Authors
**Team Byte**  
📌 *Aastha Shinde*  
📌 *Varad Dongarkar*  




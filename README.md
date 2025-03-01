# Green-Ops Hackathon: Wind Turbine SCADA Data for Early Fault Detection

## 📌 Overview
This project focuses on developing an **AI-powered predictive maintenance system** for renewable energy assets like **wind turbines and solar panels**. Using **SCADA data** and **deep learning techniques**, the system detects early signs of equipment degradation, enabling **proactive maintenance** to reduce downtime and enhance energy efficiency.

### 📂 Dataset
- **Source**: [Kaggle - Wind Turbine SCADA Data for Early Fault Detection](https://www.kaggle.com/datasets/azizkasimov/wind-turbine-scada-data-for-early-fault-detection)

---
## 🚀 Features
✅ **SCADA-Based Anomaly Detection**: Extracts key metrics such as **power output, rotor speed, and environmental conditions**.

✅ **Deep Learning for Anomaly Detection**: Utilizes **autoencoders** and **time-series models (RNNs/Transformers)** to predict failures.

✅ **Multi-Sensor Data Fusion**: Combines sensor readings to **enhance failure detection accuracy**.

✅ **Failure Prediction Modeling**: Estimates the **Remaining Useful Life (RUL)** of components for **proactive scheduling**.

---
## 🛠 Setup Instructions
### 1️⃣ Install Required Libraries:
```bash
pip install kaggle numpy pandas tensorflow scikit-learn matplotlib seaborn
```

### 2️⃣ Upload Kaggle API Key:
Upload your `kaggle.json` file.
```python
from google.colab import files
files.upload()  # Upload the kaggle.json file
```

### 3️⃣ Configure Kaggle Credentials:
```bash
mkdir -p ~/.kaggle
mv kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```

### 4️⃣ Download and Extract Dataset:
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
- Enhance **model generalization** for different asset types.
- Deploy in a **real-time monitoring system** for live anomaly detection.
- Optimize model efficiency for **lower latency predictions**.

---
## 👥 Authors
**Team Byte**  
📌 *Aastha Shinde*  
📌 *Varad Dongarkar*  

---
### 🔗 Connect
For any queries or collaboration, feel free to reach out!

📧 Email: [your-email@example.com](mailto:your-email@example.com) *(Replace with actual email if needed)*


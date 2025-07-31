🧠 Wafer Fault Detection Project


🕹️ Overview


Welcome to the Wafer Fault Detection project! This repository provides a robust, end-to-end machine learning pipeline for automatically detecting faulty wafers in semiconductor manufacturing using real sensor data. The main objective is to classify each wafer as Good (1) or Bad (-1) based on 590+ readings from the fabrication process.

Goal: Predict wafer quality in real-time for higher production yield and lower waste.

Type: Supervised Binary Classification

Tech: Python, Machine Learning, Flask, Clean Modular Architecture ⚙️

🧾 Table of Contents
📋 Problem Statement

🗂️ Project Structure

🌟 Features

🏷️ Data Details

🏁 Setup and Installation

🚦 How to Use

🔬 Project Workflow

📈 ML Approach

🤝 Contributing

📧 Contact

🏆 Acknowledgments

📋 Problem Statement
Objective: Develop a machine learning model to predict whether a semiconductor wafer is "Good" or "Bad" based on the sensor readings collected during the fabrication process.

Input: 590 sensor readings per wafer (Sensor-1, ..., Sensor-590)

Output: “Good” (1) or “Bad” (-1)

Business Impact:

Early fault detection reduces losses, increases manufacturing throughput, and enables rapid action.

🗂️ Project Structure

text

SENSORPROJECT/

├── artifacts/                    # Model artifacts, scaler, transformer, etc.
├── config/
│   └── model.yaml                # Model and pipeline configuration
├── logs/                         # Logging and error tracking
├── notebooks/
│   └── wafer_23012020_041211.csv # Sample sensor data
├── prediction_artifacts/
│   └── test.csv                  # Data or artifacts for prediction runs
├── predictions/
│   └── prediction_file.csv       # Output predictions
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   ├── constant/
│   ├── pipeline/
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   ├── utils/
│   │   ├── exception.py
│   │   └── logger.py
├── static/css/
│   └── style.css                 # Styles for web UI
├── templates/
│   └── upload_file.html
├── app.py                        # Flask web application
├── upload_data.py                # Batch upload utility
├── requirements.txt              # All dependencies
├── setup.py                      # Build details
└── README.md
🌟 Features
🔧 Modular & Clean Code: Easily extensible and production-ready Python codebase.

📊 Data Ingestion & Processing: Handles raw incoming CSV data, cleaning, scaling, and feature engineering.

🏋️♂️ Model Training: Supports a variety of classifiers (Logistic Regression, Random Forest, Gradient Boosting, Neural Networks).

🧪 Full ML Pipeline Automation: End-to-end automation from ingestion to deployment.

🖥️ Real-Time Prediction: Predict wafer quality instantly via a web interface.

📝 Robust Logging: Centralized, detailed logging and error handling.

🔁 Continuous Learning: Supports feedback loops and retraining.

☁️ Web Deployment: RESTful API via Flask (app.py) with custom HTML upload UI.

🖌️ Customizable UI: Polished CSS for an attractive file upload experience.

🏷️ Data Details
File Format: CSV (Comma-Separated Values)

Features: 590+ sensor readings per wafer (Sensor-1, Sensor-2, ..., Sensor-590)

Target: Good (1) / Bad (-1)

Example Row:

text
Wafer-801, 2968.33, 2476.58, ..., 1
🏁 Setup and Installation
1. Clone This Repo
bash
git clone https://github.com/yourgithub/wafer-fault-detection.git
cd wafer-fault-detection
2. Install Dependencies
bash
pip install -r requirements.txt
3. Setup Python Environment (Recommended)
bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
4. Configure Your Model
Edit /config/model.yaml to change pipeline or training parameters.

🚦 How to Use
🎯 Train the Model
bash
python src/pipeline/train_pipeline.py
🔮 Make Predictions (Batch or Web UI)
For command-line batch prediction:

bash
python src/pipeline/predict_pipeline.py
For web upload and instant prediction:

bash
python app.py
# Open http://127.0.0.1:5000/ in your browser
⬆️ Upload Data for Prediction
Use the provided web interface (templates/upload_file.html) to upload a CSV and see wafer predictions.

🔬 Project Workflow
Data Ingestion: Reads and validates raw wafer sensor data.

Preprocessing: Cleans NaNs, scales features, and engineers new columns if needed.

Model Training: Trains the model using multiple algorithms, selects the best based on evaluation.

Prediction: Applies the trained model to uploaded data for real-time wafer fault detection.

Continuous Update: Retrain with new production batches for higher accuracy.

📈 ML Approach
Cleaning: Removes outliers, normalizes values, imputes missing data.

Feature Engineering: Sophisticated derivation from raw sensor streams.

Model Selection: Trains and compares Logistic Regression, Random Forest, Gradient Boosting, and Neural Network models.

Evaluation: Uses Precision, Recall, F1, Confusion Matrix, etc., for assessment.

Deployment: REST API with Flask for real-time classification, easily portable for production.

🤝 Contributing
Contributions welcome!

🐛 Fix bugs

🏋️♂️ Add new models

📈 Improve evaluation or logging

💡 Suggest or implement UI improvements

Fork the repo, make your changes, and create a pull request. All feedback is appreciated!

📧 Contact
Made with ❤️ by Om

Email:omk99919@gmail.com

GitHub:https://github.com/omkumar23112003

🏆 Acknowledgments
Special thanks to the open-source & data science community.

Kaggle and open datasets for inspiration.

This project demonstrates a complete, scalable machine learning workflow for semiconductor wafer fault detection, maximizing reliability and production-grade deployment. Explore, contribute, and help build better chips!

README last updated: Aug 01, 2025 — Om

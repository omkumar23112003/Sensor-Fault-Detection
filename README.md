🛠️ Sensor Fault Detection Machine Learning Project
📢 Overview
This project implements an end-to-end Machine Learning pipeline for real-time wafer sensor fault detection.
It uses automated data ingestion, preprocessing, model training & selection, and provides an interactive prediction interface via a Flask-based web app.

The goal is to help manufacturers quickly determine whether wafers from sensor readings are faulty or normal, ensuring high-quality production and reducing defects.

🚀 Features
Upload Data for Prediction:
Web interface to upload CSV sensor data and instantly get predictions.

Complete ML Pipeline:

Data ingestion and validation

Data cleaning, scaling, and feature engineering

Multiple model training & best model selection

Real-time prediction on uploaded data

Continual model retraining for improved accuracy

Multiple Algorithms Tested: Logistic Regression, Random Forest, Gradient Boosting, Neural Networks

Robust Model Evaluation: Precision, Recall, F1-score, and Confusion Matrix.

📈 Machine Learning Approach
Data Cleaning

Remove outliers and noisy readings

Normalize data for consistent scaling

Handle missing values via imputation

Feature Engineering

Create derived features from raw sensor streams

Select most relevant features using statistical methods or feature importance

Model Training & Selection

Train Logistic Regression, Random Forest, Gradient Boosting, and Neural Network models

Compare using evaluation metrics

Automatically select the best-performing model

Evaluation Metrics

Precision, Recall, F1-score, Accuracy

Confusion Matrix to analyze classification results

Real-time Prediction

Upload any new CSV via a web form

Instant prediction of wafer status (Faulty / Normal)

🗂️ Project Structure
text
SENSORPROJECT/
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   ├── model_trainer.py
│   ├── pipeline/
│   │   ├── predict_pipeline.py
│   │   ├── train_pipeline.py
│   ├── utils/
│   │   ├── exception.py
│   │   ├── logger.py
│   ├── constant/
│   ├── static/
│   │   ├── style.css
│   ├── templates/
│   │   ├── upload_file.html
│   ├── app.py
│   ├── upload_data.py
│
├── requirements.txt
├── setup.py
├── README.md
└── ...
💾 Installation & Setup
Clone the Repository

bash
git clone https://github.com/yourusername/sensor-fault-detection.git
cd sensor-fault-detection
Install Dependencies

bash
pip install -r requirements.txt
Run the Flask Web App

bash
python app.py
Open http://localhost:5000 in a browser to access the upload form and start predictions.

⚡ Key Results & Insights
High detection accuracy reducing defective wafers from passing QA.

Automatic best model selection allowing optimized performance for any dataset.

Continuous learning through retraining with new incoming data batches.

Detailed error analysis using Confusion Matrix to identify common misclassifications.

📍 Future Scope
Real-time Streaming: Add live sensor data intake for continuous predictions.

API Deployment: Expose predictions via a REST API for integration into other systems.

Advanced Models: Integrate deep learning approaches like LSTM for time-series sensor data.

Cloud Deployment: Host on AWS/GCP/Azure for remote access and scalability.

Interactive Dashboards: Build visualization dashboards showing live predictions and stats.

Data Security Enhancements: Encrypt sensitive sensor data in transit and storage.

🙌 Acknowledgements
Open-source community for Python, Flask, and ML libraries.

Sensor dataset providers for wafer reading examples.

Developers of Scikit-learn, NumPy, Pandas, and Matplotlib for core tools.

📧 Contact
For support, collaboration, or questions, reach out via email:
omk99919@gmail.com

📜 License
This project is licensed under the MIT License — you may use, modify, and distribute it with attribution.
See the LICENSE file for details.

<img width="1252" height="796" alt="image" src="https://github.com/user-attachments/assets/01df7749-f762-4272-abca-a3090bf6e9bd" />


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

<img width="687" height="619" alt="image" src="https://github.com/user-attachments/assets/9e638117-ad34-44ca-8b4b-76dfd05b20d6" />

🧰 Tech Stack for Sensor Fault Detection Machine Learning Project
Programming Languages
Python 3.x — Core programming language for ML model development and web app.

Machine Learning Libraries
Scikit-learn — Model training, evaluation, and selection.

TensorFlow / Keras or PyTorch (if using neural networks).

NumPy — Numerical computations.

Pandas — Data manipulation and preprocessing.

Matplotlib / Seaborn — Visualization of data and model results.

Data Engineering & Processing
SQL (if any database use for storing sensor or prediction results)

Pandas for ETL (Extract, Transform, Load operations on sensor data)

Web Framework
Flask — Lightweight web application framework for the upload and prediction interface.

Frontend
HTML/CSS — For web interface (upload_file.html)

Optionally, Bootstrap or similar CSS frameworks for responsive UI.

DevOps & Deployment (optional/for future scope)
Docker — Containerization for easy deployment.

AWS/GCP/Azure — Cloud platform for hosting and scalability.

RESTful API frameworks (Flask-RESTful or FastAPI) if developing service APIs.

Version Control & Collaboration
Git & GitHub — Source code versioning and collaboration.

Other Tools & Utilities
Jupyter Notebook — Development and experimentation environment.

Logging — Python logging module or custom logger for debugging and error handling.

Data Validation — Custom scripts or libraries to ensure data quality.


⚡ Key Results & Insights
High detection accuracy reducing defective wafers from passing QA.

Automatic best model selection allowing optimized performance for any dataset.

Continuous learning through retraining with new incoming data batches.

Detailed error analysis using Confusion Matrix to identify common misclassifications.

<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/90a95605-4123-422b-87b7-b454c304094d" /><img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/6e125818-85d4-48f7-9238-a78b170e1433" />



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

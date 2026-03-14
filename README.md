# AI-Based Anomaly Detection in Patient Health Monitoring using Kafka Streaming

## Project Overview

This project implements a **real-time patient health monitoring system** that detects abnormal health conditions using streaming data and machine learning.

The system streams patient vitals data through Apache Kafka, processes it in real time, detects anomalies, and visualizes results on a dashboard.

## Technologies Used

- Apache Kafka â€“ Real-time data streaming
- Python â€“ Core programming language
- Flask â€“ Backend API
- Streamlit â€“ Dashboard visualization
- Scikit-learn â€“ Machine learning for anomaly detection
- Pandas â€“ Data processing

## System Architecture

Patient Data Generator  
â†“  
Kafka Producer  
â†“  
Kafka Topic (patient-vitals)  
â†“  
Kafka Consumer  
â†“  
Patient Monitoring + Alert Detection  
â†“  
CSV Data Storage  
â†“  
Flask API  
â†“  
Streamlit Dashboard

## Project Structure

AI-Anomaly-Detection/

producer.py â€“ Sends patient vitals to Kafka  
consumer.py â€“ Receives data and processes alerts  
train_model.py â€“ Trains anomaly detection model  
patient_data.csv â€“ Dataset generated from streaming  

backend/  
app.py â€“ Flask API  

dashboard/  
dashboard.py â€“ Streamlit dashboard  

model/  
anomaly_model.pkl â€“ Trained ML model  

requirements.txt â€“ Project dependencies  
README.md â€“ Project documentation

## Features

- Real-time patient vitals streaming
- Kafka-based event processing
- Patient monitoring system
- Explainable health alerts
- AI-based anomaly detection
- Interactive dashboard visualization

## Installation

1. Clone or download the project.

2. Install dependencies:

pip install -r requirements.txt

3. Download and extract Apache Kafka.

4. Start Kafka server.

## Running the Project

Step 1: Start Kafka server

bin/windows/kafka-server-start.bat config/server.properties

Step 2: Run Producer

python producer.py

Step 3: Run Consumer

python consumer.py

Step 4: Run Backend API

python backend/app.py

Step 5: Run Dashboard

streamlit run dashboard/dashboard.py

## Output

The system will show:

- Real-time patient health data
- Alert messages for abnormal vitals
- Health monitoring dashboard with graphs

## Example Alert

âš  ALERT for Patient 2  
Reasons:  
- High Heart Rate  
- Low Oxygen

## Future Improvements

- Integration with real hospital IoT devices
- Deep learning anomaly detection
- Cloud deployment
- Mobile health monitoring app

## Author

Rishank Singh  
AI-Based Health Monitoring Project

## Adaptive Network Intrusion Detection System

### Project Overview
This project implements a backend system focused on the continuous analysis and detection of network traffic anomalies. By leveraging machine learning techniques, the system automatically detects **concept drift** and adapts the model using a **warm-up/recent data window strategy**, ensuring it remains effective over time as network traffic patterns evolve.

### Key Features
- **Concept Drift Detection:**  
  The system identifies concept drift, a phenomenon where the underlying data distribution changes over time, and triggers the adaptation of the machine learning model accordingly. This is achieved through a warm-up and recent data window strategy that continuously updates the model to stay aligned with the most recent data patterns.

- **Automated Model Retraining:**  
  To enhance the model's robustness, centroid-based unsupervised monitoring is used. This monitoring method triggers the retraining of the **XGBoost** model on **CIC-IDS2017** network traffic data, ensuring the system adapts to new types of anomalies and evolving network behavior.

- **Real-Time Model Adaptation:**  
  The system ensures real-time detection and automatic retraining without manual intervention, maintaining optimal detection accuracy even as new data arrives.

### Tech Stack
- **Languages & Libraries:** Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib  
- **Platform:** Google Colab (for model development and training)

### Additional Features
- **Data Preprocessing:**  
  Utilizes Pandas and NumPy for efficient data manipulation, cleaning, and preparation before model training.
  
- **Visualization:**  
  Leverages Matplotlib for visualizing model performance and monitoring the detection of concept drift.

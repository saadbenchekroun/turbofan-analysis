# Platform for Analysis, Visualization, and Processing of Turbofan Engine Data

## Overview

This platform is designed for analyzing, visualizing, and processing turbofan engine data. The data is sourced from NASA’s Turbofan Engine Degradation Simulation Dataset (CMAPSS). The platform offers insights into key engine performance metrics, predictions for remaining useful life (RUL), and leverages machine learning models to support predictive maintenance and operational efficiency.

## Key Features

- **Data Visualization and Insights**:  
  Provides advanced visualizations and real-time dashboards for engine sensor data, including metrics such as engine pressure ratio (EPR), fuel flow ratio, and more.

- **KPI Calculation**:  
  Node.js backend enables real-time computation of Key Performance Indicators (KPI) like engine reliability, availability, and overall health.

- **Machine Learning Integration**:  
  Integrates an LSTM (Long Short-Term Memory) model to predict the remaining useful life (RUL) of turbofan engines using the NASA dataset.

- **Vectorized Data Management**:  
  Utilizes SingleStore as a scalable vector database for efficient embedding storage and retrieval, optimizing search queries on large sensor datasets.

- **Google Cloud Platform (GCP)**:  
  Leverages Vertex AI API for enhanced data processing and enrichment, providing deeper insights from raw sensor data.

- **Natural Language Data Analysis**:  
  Integration with OpenAI’s API allows querying sensor data in natural language for tasks such as anomaly detection and sensor failure predictions.

## Tech Stack

- **Frontend**:  
  Developed using React.js to ensure a dynamic and interactive user interface with a focus on real-time data visualization.

- **Backend**:  
  - **Node.js**: Manages KPI calculations and serves data to the frontend.  
  - **Flask**: Powers machine learning workflows, including data preprocessing and the LSTM model for predictive analytics.

- **Database**:  
  SingleStore is used as the primary storage for sensor data embeddings, enabling efficient real-time analysis.

- **Machine Learning**:  
  - **LSTM Model**: Utilized for time-series predictions, specifically to estimate the remaining useful life of turbofan engines.  
  - **Vertex AI (GCP)**: Facilitates data enrichment and machine learning model deployment.

- **APIs**:  
  - **OpenAI API**: Provides advanced natural language-based data analysis capabilities.

## Usage

- **Data Upload**:  
  Users can upload new sensor data via the frontend. The data is processed and embedded in the vector database.

- **KPI Monitoring**:  
  The platform calculates and displays real-time KPIs for engine performance, reliability, and health.

- **Predictive Maintenance**:  
  The LSTM model analyzes sensor data to predict the remaining useful life of the engines.

- **Natural Language Insights**:  
  Query sensor data through a chatbot interface that leverages OpenAI's API for dynamic analysis and predictive insights.

## Data

The data used in this project is sourced from NASA’s Commercial Modular Aero-Propulsion System Simulation (CMAPSS) dataset. It simulates degradation in turbofan engines and provides valuable insights for predictive maintenance.

## Contributions

We welcome contributions! Please open an issue or submit a pull request if you'd like to help improve the platform.

## License

This project is licensed under the MIT License.

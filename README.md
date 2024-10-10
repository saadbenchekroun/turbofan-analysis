Platform for Analysis, Visualization, and Processing of Turbofan Engine Data

#Overview#

This repository contains the codebase for a highly specialized platform designed for analyzing, visualizing, and processing data from turbofan engines. The data utilized in this project is sourced from NASA’s Turbofan Engine Degradation Simulation Dataset (CMAPSS). The platform provides insights into key engine performance metrics, predictions for remaining useful life (RUL), and leverages machine learning models to support predictive maintenance and operational efficiency.

#Key Features#

##Data Visualization and Insights:## Advanced visualizations and real-time dashboards for engine sensor data, including metrics like engine pressure ratio (EPR), fuel flow ratio, and more.

##KPI Calculation:## Node.js backend for real-time computation of Key Performance Indicators (KPI) such as engine reliability, availability, and overall health.

##Machine Learning Integration:## The platform integrates an LSTM (Long Short-Term Memory) model to predict the remaining useful life (RUL) of turbofan engines based on the NASA dataset.

##Vectorized Data Management:## Uses SingleStore as a scalable vector database for efficient embedding storage and retrieval, optimizing search queries on large sensor datasets.

##Google Cloud Platform (GCP):## Utilizes Vertex AI API for enhanced data processing and enrichment, providing additional context to the raw sensor data for deeper insights.

##Natural Language Data Analysis:## Integration with OpenAI’s API allows advanced querying of sensor data for natural language-driven insights, such as anomaly detection or sensor failure predictions.


#Tech Stack#

##Frontend:## Developed using React.js, ensuring a dynamic and interactive user interface with a focus on real-time data visualization and performance.

##Backend:##

###Node.js:### Manages the calculation of KPI metrics and serves data to the frontend.

###Flask:### Powers the machine learning workflows, including data preprocessing and the LSTM model for predictive analytics.


###Database:### SingleStore serves as the primary storage for sensor data embeddings, enabling efficient queries for real-time analysis.

##Machine Learning:##

###LSTM Model:### Used for time-series predictions, particularly for estimating engine remaining useful life (RUL).

###Vertex AI (GCP):### Facilitates data enrichment and ML model deployment.


##APIs:##

OpenAI API: Provides advanced, natural language-based data analysis capabilities.





#Usage#

##Data Upload:## Users can upload new sensor data via the frontend. The data is then processed and embedded in the vector database.

##KPI Monitoring:## The platform automatically calculates and displays real-time KPIs for engine performance, reliability, and health.

##Predictive Maintenance:## The LSTM model analyzes sensor data to predict the remaining useful life of the engines.

##Natural Language Insights:## Query sensor data through a chatbot interface that leverages the OpenAI API for dynamic analysis and predictive insights.


#Data#

The data used in this project comes from NASA’s Commercial Modular Aero-Propulsion System Simulation (CMAPSS) dataset. This dataset simulates degradation in turbofan engines and provides valuable insights for predictive maintenance.

#Contributions#

We welcome contributions! Please open an issue or submit a pull request if you'd like to help improve the platform.

#License#

This project is licensed under the MIT License.

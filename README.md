# SBA_AnomalyDetection

This repository contains a project focused on **streaming anomaly detection** using the **Statistical Bayesian ARIMA algorithm**.

## Overview
The goal of this project is to perform anomaly detection on streaming time-series data. The model utilizes **BAYESIAN ARIMA** (AutoRegressive Integrated Moving Average), with the ability to dynamically update the model as new data arrives via Kafka streams.

## Instructions to Run the Code


1. **Run in Jupyter Notebook**:
   - You can run the code in a Jupyter notebook or Google Colab. The notebook should be executed **line by line**.

### Running the Code:
1. Launch Jupyter Notebook and open the main notebook in the repository.
   
2. Once you run, you will be prompted to provide the path of one of the available datasets.
- When prompted, provide the path to the dataset. For example: realKnownCause/nyc_taxi.csv (This is necessary because the code uses **Kafka** to stream the CSV file inputs dynamically and then train the model in a **streaming fashion**)
- The Kafka stream will send chunks of the data to the model, allowing it to train incrementally and detect anomalies in real-time.

### Dataset Options:
You can choose from different pre-defined datasets stored in the **dataset** folder of the repository 
 

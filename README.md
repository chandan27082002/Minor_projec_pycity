# Minor_projec_pycity

# Electricity Consumption Forecasting Using PyCity — Mini Project

This project presents an end-to-end workflow for forecasting electricity consumption using a synthetic dataset generated with pycity_base. The dataset contains hourly electricity usage for the year 2024, enabling structured analysis, feature exploration, and model development.


# 📊 Project Overview

The workflow covers the complete pipeline:

Synthetic data generation using pycity_base

Exploratory Data Analysis (EDA)

Time-series decomposition and stationarity checks

Baseline and advanced forecasting models

Performance evaluation using multiple metrics

Through EDA, the dataset showed daily and weekly seasonal patterns, along with a moderately right-skewed distribution and no outliers. Time-series decomposition revealed strong weekly seasonality and minor mid-year fluctuations. Stationarity tests confirmed that the series is suitable for autoregressive modeling.

Autocorrelation and partial autocorrelation analyses highlighted short-term dependencies and repeating cycles, supporting the use of both classical statistical models and deep learning models.

# 🤖 Modeling & Results

Several forecasting models were implemented:

Naive Baseline Model

AR(1) Autoregressive Model

Vanilla RNN

LSTM

GRU

Key findings:

The Naive model provided a basic benchmark with limited predictive capability.

The AR(1) model achieved strong performance with R² > 0.98.

Deep learning models—especially GRU—captured nonlinear temporal patterns effectively.

The GRU model performed best, achieving R² > 0.995, demonstrating superior accuracy and robustness.

# 🧠 Conclusion

This project shows that while simple autoregressive models perform well on stationary datasets, advanced recurrent neural networks (RNNs) such as GRU, LSTM, and RNN provide higher accuracy and stronger generalization for electricity demand forecasting.

The workflow established here serves as a foundation for scaling to multi-building, district-level, or full city-level forecasting, enabling smarter energy planning and management.

# 🚀 Future Scope

Although the current project focuses on a single building, there is substantial scope for expansion.

# 🏙️ 1. City-Scale Synthetic Data Generation

Using the full pyCity ecosystem (pycity_base, pycity_calc, pycity_street), future work can include:

Extracting building geometry and street networks from OpenStreetMap

Assigning building types, occupancy behavior, and appliance models

Simulating hourly electricity loads for entire districts or cities

Aggregating data for forecasting at building, feeder, district, or city level

This enables creation of realistic, high-resolution urban energy datasets.

# 🔧 2. Handling Missing or Incomplete Real Data

Synthetic data can be used to:

Fill gaps in real-world sensor measurements

Create long sequences needed for deep learning

Provide benchmark datasets

Improve model generalization and robustness

This is especially helpful when real datasets have noise or missing timestamps.

# 🏘️ 3. Multi-Building and City-Level Forecasting

The workflow can scale from a single building to:

Residential colonies or multi-building clusters

Feeder-level and district-level forecasting

City-wide predictions using hierarchical modeling with pyCity

This scalability makes pyCity suitable for smart grid applications and urban energy planning.

# 📌 Summary

Future development will extend this project into urban-scale load forecasting, integrating synthetic and real data for better accuracy and practical usability. With pyCity tools, the project can evolve towards:

Smart city energy modeling

District-level consumption simulation

Data-driven energy management strategies

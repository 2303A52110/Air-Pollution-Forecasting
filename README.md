# 🌍 Deep Learning Approaches for Air Pollution Forecasting Based on Explainable AI

<div align="center">

### Predicting PM2.5 Concentration using LSTM, GRU, CNN-LSTM and Explainable AI

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=for-the-badge&logo=tensorflow)
![Deep Learning](https://img.shields.io/badge/Deep-Learning-red?style=for-the-badge)
![Explainable AI](https://img.shields.io/badge/XAI-SHAP%20%7C%20LIME-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

### Building Accurate and Trustworthy Air Quality Forecasting Systems Through Deep Learning & Explainable AI

</div>

---

# 📖 Overview

Air pollution remains one of the most critical environmental and public health challenges worldwide. Accurate forecasting of air quality enables governments, healthcare organizations, and citizens to take proactive measures against hazardous pollution events.

This project presents a **Deep Learning-based Air Pollution Forecasting Framework** that predicts **PM2.5 concentrations** using historical environmental and meteorological data from Beijing's PRSA Air Quality Dataset.

The framework combines:

- 🧠 Deep Learning Models (LSTM, GRU, CNN-LSTM)
- 📊 Time-Series Forecasting
- 🔍 Explainable AI (SHAP & LIME)
- 🌡️ Meteorological Feature Analysis
- 📈 Environmental Data Analytics

The goal is not only to achieve high predictive accuracy but also to make model decisions transparent and interpretable.

---

# 🎯 Objectives

- Forecast PM2.5 concentration levels accurately
- Learn temporal pollution patterns from historical data
- Compare multiple Deep Learning architectures
- Identify environmental factors influencing air quality
- Improve transparency using Explainable AI techniques
- Support future smart-city and public-health applications

---

# 🏗️ System Architecture

```text
Air Quality Dataset
        │
        ▼
Data Cleaning & Preprocessing
        │
        ▼
Feature Engineering
        │
        ▼
Time-Series Sequence Generation
        │
        ▼
Deep Learning Models
 ┌─────────────┐
 │    LSTM     │
 ├─────────────┤
 │     GRU     │
 ├─────────────┤
 │  CNN-LSTM   │
 └─────────────┘
        │
        ▼
PM2.5 Forecasting
        │
        ▼
SHAP + LIME Explanations
```

---

# 📊 Dataset

## Dataset Source

**PRSA Beijing Air Quality Dataset**

## Time Period

**2010 – 2014**

## Target Variable

- PM2.5 Concentration (µg/m³)

## Input Features

### Pollution Features

- PM2.5

### Meteorological Features

- Temperature (TEMP)
- Dew Point (DEWP)
- Atmospheric Pressure (PRES)
- Wind Speed (Iws)
- Wind Direction (cbwd)
- Precipitation
- Snowfall

---

# 🧹 Data Preprocessing

The dataset undergoes multiple preprocessing steps before training:

### Missing Value Handling

- Removal of invalid PM2.5 entries
- Linear interpolation for missing meteorological values

### Outlier Detection

- Extreme pollution values identified using IQR methods
- Noise reduction and anomaly correction

### Feature Engineering

- Min-Max Normalization
- One-Hot Encoding for Wind Direction
- Time-Series Sequence Generation

### Dataset Splitting

- Training Set → 70%
- Validation Set → 15%
- Testing Set → 15%

---

# 🧠 Deep Learning Models

## 1️⃣ Long Short-Term Memory (LSTM)

LSTM networks effectively capture long-term temporal dependencies within pollution data.

### Advantages

- Handles sequential data efficiently
- Learns long-range dependencies
- Excellent forecasting performance

---

## 2️⃣ Gated Recurrent Unit (GRU)

A lightweight alternative to LSTM with fewer parameters.

### Advantages

- Faster training
- Reduced computational cost
- Strong forecasting capability

---

## 3️⃣ CNN-LSTM Hybrid

Combines spatial feature extraction and temporal learning.

### Advantages

- Captures feature interactions
- Learns temporal patterns
- Suitable for spatio-temporal forecasting

---

# 🔍 Explainable AI (XAI)

One of the biggest challenges in Deep Learning is model interpretability.

To address this challenge, this project integrates:

## SHAP (SHapley Additive Explanations)

Provides:

- Global Feature Importance
- Feature Contribution Analysis
- Model Transparency

## LIME (Local Interpretable Model-Agnostic Explanations)

Provides:

- Local Prediction Explanations
- Event-Specific Interpretability
- Decision Understanding

Together, SHAP and LIME transform black-box models into transparent and trustworthy forecasting systems.

---

# 📈 Model Performance

| Model | MAE | RMSE | R² Score | Pearson Correlation |
|---------|---------|---------|---------|---------|
| **LSTM** | **8.42** | **11.27** | **0.92** | **0.94** |
| **GRU** | 9.15 | 12.03 | 0.90 | 0.92 |
| **CNN-LSTM** | 8.76 | 11.63 | 0.91 | 0.93 |

## 🏆 Best Model

### LSTM

The LSTM model achieved:

- Lowest MAE
- Lowest RMSE
- Highest R² Score
- Strongest Correlation with Observed Values

---

# 🌡️ Key Findings

## Factors Increasing PM2.5 Levels

- High Temperature
- High Dew Point
- Unfavorable Wind Direction

## Factors Reducing PM2.5 Levels

- Strong Wind Speed
- High Atmospheric Pressure

The Explainable AI analysis confirmed that the model learned scientifically meaningful environmental relationships.

---

# 📷 Visualizations

## Daily PM2.5 Time Series

Tracks pollution fluctuations over time and identifies major pollution spikes.

## PM2.5 Heatmap

Visualizes average pollution levels across locations and months.

## Temperature vs PM2.5 Correlation

Analyzes the influence of temperature on pollution concentration.

## Monthly Distribution Analysis

Examines seasonal pollution behavior.

## Yearly PM2.5 Trends

Shows long-term pollution evolution between 2010 and 2014.

---

# 🚀 Technology Stack

## Programming Language

- Python

## Data Analysis

- Pandas
- NumPy

## Visualization

- Matplotlib
- Seaborn

## Machine Learning

- Scikit-Learn

## Deep Learning

- TensorFlow
- Keras

## Explainable AI

- SHAP
- LIME

## Development Environment

- Jupyter Notebook
- Google Colab

---

# 📂 Project Structure

```text
Air-Pollution-Forecasting/
│
├── dataset/
│   └── PRSA_Data.csv
│
├── notebooks/
│   └── Air_Pollution_Forecasting.ipynb
│
├── images/
│   ├── Daily_PM25.png
│   ├── PM25_Heatmap.png
│   ├── Correlation.png
│   ├── Distribution.png
│   └── Yearly_Trends.png
│
├── research_paper/
│   └── Air_Pollution_Forecasting.pdf
│
├── requirements.txt
└── README.md
```

---

# 📊 Results

✅ Accurate PM2.5 Forecasting

✅ Time-Series Learning

✅ Explainable AI Integration

✅ Environmental Feature Analysis

✅ State-of-the-Art Deep Learning Models

✅ Research-Oriented Implementation

---

# 🔬 Future Enhancements

- Transformer-Based Forecasting
- Temporal Fusion Transformers (TFT)
- Graph Neural Networks (GNN)
- Real-Time Air Quality Prediction
- Satellite Data Integration
- Edge AI Deployment
- Smart City Applications
- IoT-Based Monitoring Systems

---

# 🏆 Project Highlights

✔ Deep Learning Based Forecasting

✔ Explainable AI Integration

✔ Research-Oriented Implementation

✔ Real Environmental Dataset

✔ Public Health Applications

✔ Smart City Potential

✔ Time-Series Forecasting

✔ Environmental Analytics

---

<div align="center">

### 🌍 Building Smarter and More Transparent Air Quality Forecasting Systems Through Deep Learning and Explainable AI

</div>

# Forecasting Pothole Development in Syracuse, NY

This repository contains the final project for IST 707 Applied Machine Learning course, Syracuse University. Our project aims to forecast pothole development in Syracuse, NY, based on multiple factors such as weather, pavement ratings, and reported maintenance requests.

## Problem Statement

Pothole development occurs due to:
- Poor paving materials.
- Extreme temperature changes.
- Traffic load over time.

This leads to road deterioration, impacting road safety and maintenance costs.

## Goal

To build a predictive model that:
- **Forecasts the count of potholes**.
- Helps **city maintenance departments** to efficiently plan maintenance operations.
- **Reduces costs** and improves road safety.

---

## **Data Sources**

We utilized several public datasets relevant to road conditions, weather, and maintenance requests:

### 1. **Pavement Ratings Data**  
   Data provided by the **Syracuse Metropolitan Transportation Council** across multiple years:
   - [**2021 Pavement Ratings**](https://data.syr.gov/datasets/4fd187e47c59492cabf55344beb8d538_0/explore?location=43.034839%2C-76.140694%2C12.76)  
   - [**2022 Pavement Ratings**](https://data.syr.gov/maps/4f7775b13afa4227a772124edfb610fc/about)  
   - [**2023 Pavement Ratings**](https://data.syr.gov/datasets/442deefc49b2494c8cc5708e36c06cdb_0/explore?location=43.034839%2C-76.140694%2C12.76)  

### 2. **Weather Data**  
   Weather data from **NASA**, capturing climate conditions such as temperature fluctuations and precipitation, which impact road quality.  

### 3. **SYRCityline Requests Data**  
   Collected by Syracuse citizens via **SeeClickFix**, this dataset tracks public maintenance requests, including pothole reports.  
   - [**SYRCityline Requests**](https://data.syr.gov/datasets/0d58a53ccb22457990161d756ed8a870_0/explore)  

### 4. **Streets Database**  
   Detailed street information from Syracuse’s open data portal. This dataset provides road classifications and usage patterns that help predict pothole-prone areas.  
   - [**Syracuse Streets Data**](https://data.syr.gov/datasets/47cadd4fe5b344f895c5a3e672463899_0/explore)  

Data collected from **2021-2023**.

---

## Project Overview

1. **EDA (Exploratory Data Analysis):**
   - Correlation matrices and visual insights.
   
2. **Model:** 
   - **Linear Regression** (Baseline)
   - Loss function: Mean Squared Error (MSE)

3. **Data Preprocessing:**
   - **Numerical Features:** Imputed with the mean and scaled.
   - **Categorical Features:** Imputed with the most frequent value, one-hot encoded.

4. **Data Split:**
   - Train: 60%
   - Validation: 20%
   - Test: 20%

---

## Repository Structure

- `/data/`: Contains raw and processed datasets.
- `/notebooks/`: Jupyter notebook with code and experiments.
- `/src/`: Scripts for preprocessing, training, and evaluation.
- `/models/`: Saved model weights and checkpoints.
- `/presentation/`: Final project presentation in PPT format.

---

## Results

Our linear regression model achieved:

- **MSE (Mean Squared Error):** <value to be updated>
- <Add any key insights or findings from your results>

---

## Installation

To set up the environment, use:

```bash
pip install -r requirements.txt

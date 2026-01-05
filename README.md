# Airfare Price Prediction Using Machine Learning

**Academic Mini Project (Semester 3.2)**  
**Project Duration:** February 2025 – June 2025  

---

## Overview
Airfare Price Prediction is a machine learning–based system designed to estimate the **approximate price of domestic airline tickets** based on user-provided travel parameters.  
The system predicts airfare using historical flight data and learned pricing patterns rather than real-time pricing rules.

A key objective of this project is to support **long-term price estimation**, allowing predictions for future travel dates — including years far ahead (e.g., 2030–2050) — based on trends learned from historical data.

---

## Problem Statement
Airfare prices are influenced by multiple factors such as airline, route, travel time, duration, and number of stops.  
Due to the dynamic nature of airline pricing, passengers often lack insight into how these factors collectively impact ticket prices over time.

This project addresses the problem by developing a **data-driven regression model** capable of predicting airfare values for both near-term and long-term travel planning scenarios.

---

## Objectives
- Build a machine learning model for airfare price estimation  
- Enable **future-year predictions** based on historical pricing patterns  
- Analyze key factors influencing airfare pricing  
- Develop a user-friendly web interface for fare prediction  
- Apply regression-based machine learning techniques to real-world data  

---

## Scope of the Project
- Applicable **only to domestic flights within India**  
- Designed for **long-term and future price estimation**  
- Predictions are generated based on learned historical trends  
- The model does not restrict year input and can process travel dates far in the future  
- Intended for analytical and planning purposes  

---

## Dataset
- **Source:** Publicly available flight fare dataset (Kaggle)  
- **Data Volume:**
  - Training samples: ~10,683  
  - Test samples: ~2,671  

### Key Features
- Airline  
- Date of Journey  
- Source (Departure Location)  
- Destination  
- Route  
- Departure Time  
- Arrival Time  
- Duration  
- Total Stops  
- Additional Information  
- Target Variable: Airfare Price  

---

## Methodology

### Data Preprocessing
- Handling missing and inconsistent data  
- Feature extraction from date and time attributes  
- Numerical representation of journey duration  
- Encoding of categorical features using one-hot encoding  

---

### Exploratory Data Analysis
- Identification of fare variation across routes and airlines  
- Analysis of factors influencing long-term pricing behavior  
- Visualization of relationships between flight attributes and price  

---

### Model Development
The following regression models were evaluated:
- Random Forest Regressor ✅ *(Final Model)*  
- Decision Tree Regressor  
- Support Vector Machine  
- XGBoost  

The **Random Forest Regressor** was selected due to its robustness, ability to model non-linear relationships, and stable performance on structured data.

---

## Final Model
- **Algorithm:** Random Forest Regressor  
- **Model File:** `flight_rf.pkl`  

The model generalizes learned pricing patterns and is capable of producing **reasonable price estimates for future travel dates**, including long-term horizons.

---

## System Implementation
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Web Framework:** Flask  

The web application allows users to input:
- Departure location  
- Destination  
- Journey date (including future years)  
- Airline  
- Number of stops  

The system processes these inputs and outputs an **estimated airfare value**.

---

## Testing
- Unit testing for individual components  
- Integration testing across modules  
- End-to-end system testing  
- Black-box and white-box testing techniques  

---

## Key Observations
- Route, airline, duration, and number of stops strongly influence airfare  
- Tree-based regression models provide stable predictions  
- The system supports both short-term and long-term travel planning scenarios  

---

## Limitations
- Predictions are based on historical data patterns  
- Applicable only to domestic flights  
- Real-time airline pricing strategies are not considered  

---

## Future Enhancements
- Incorporation of real-time flight and demand data  
- Expansion to international routes  
- Inclusion of external factors such as seasonality and economic indicators  
- Use of advanced ensemble and deep learning techniques for improved long-term forecasting  

---

## Project Contribution Note
This project was completed as a **team-based academic mini project** during Semester 3.2.  
The repository is maintained for **academic documentation, technical demonstration, and professional portfolio purposes**.

---

## Conclusion
The Airfare Price Prediction system demonstrates how machine learning can be applied to estimate flight prices using historical trends.  
By enabling **future-year predictions**, the project supports long-term travel planning and analytical exploration of airfare behavior.  
With enhanced datasets and real-time integration, the system can be extended to deliver more accurate and scalable predictions.

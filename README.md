#  Food Delivery Time Prediction using Machine Learning

##  1. Problem Statement
Food delivery platforms want to predict how long it will take for food to be delivered, so customers get accurate delivery time estimates.

Your goal is to build a regression model that predicts the **Time_taken (min)** for each food order using available features such as delivery distance, vehicle type, weather conditions, etc.

---

## 2. Dataset Description

- Dataset contains real-world delivery data with the following columns:
  - `Delivery_person_Age`
  - `Delivery_person_Ratings`
  - `Restaurant_latitude`, `Restaurant_longitude`
  - `Delivery_location_latitude`, `Delivery_location_longitude`
  - `Vehicle_condition`, `Weather_conditions`, `Traffic_density`
  - `Time_taken (min)` (Target variable)

---

##  3. Exploratory Data Analysis (EDA)

- Checked for missing values and handled them.
- Explored correlations and plotted visualizations for:
  - Delivery time vs traffic
  - Delivery ratings vs time
  - Delivery location distances

 Example Plots:
- Correlation heatmaps
- Delivery time distributions
- Traffic density comparisons

---

##  4. Feature Engineering

- Converted timestamps and locations into useful numeric features.
- Calculated **distance** using Haversine formula.
- Encoded categorical variables (e.g., Weather, Vehicle Type).
- Scaled numeric features.

---

##  5. Model Building

Trained multiple ML regression models:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor

---

##  6. Conclusion

### What did you learn?
- Features like **distance, weather, traffic, and delivery ratings** significantly affect delivery time.
- ML models can reliably predict delivery time within a reasonable error margin.

### Business-level Conclusion
- This model can help food delivery apps (like Swiggy/Zomato) give accurate **ETA predictions** to users.
- Can improve customer trust and logistics planning.

---

##  Future Work

- Include real-time GPS tracking and dynamic traffic data.
- Try deep learning models (LSTM/GRU) for time-series prediction.
- Deploy as a Flask or Streamlit-based web app.

---

##  Tools Used

| Tool | Purpose |
|------|---------|
| Python | Core programming |
| Pandas | Data manipulation |
| Matplotlib, Seaborn | Visualization |
| Scikit-learn | ML models |
| XGBoost | Advanced regression |
| Jupyter Notebook | Development environment |


---

##  How to Run

```1. Clone this repo
2. Open `food_delivery_model.ipynb` in Jupyter
3. Run all cells in order


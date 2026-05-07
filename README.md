<p align="center">
  <img src="images/kurt.jpeg" alt="Project Banner"/>
</p>

# 📊 What Drives the Price of a Car?

## 📌 Overview

This project is part of **Module 11** of the **Berkeley Professional Certificate in Machine Learning and Artificial Intelligence**.

The objective of this project is to identify the key factors that influence used car prices and develop a predictive model capable of estimating vehicle value based on available features. By analyzing characteristics such as vehicle age, mileage, manufacturer, fuel type, condition, transmission, and title status, the project aims to help used car dealerships better understand pricing behavior in the market.

---

## 📂 Dataset

The original dataset contained information on approximately 3 million used cars. The provided dataset includes information on approximately 426,000 vehicles to improve processing efficiency.

The dataset contains the following information:

- Vehicle price
- Manufacturer
- Model
- Year
- Odometer mileage
- Fuel type
- Transmission
- Vehicle condition
- Title status
- Drive type
- Vehicle type
- Region
- State

Several preprocessing and cleaning steps were required before modeling due to missing values, outliers, inconsistent categories, and skewed distributions.

---

## 🛠️ Data Preparation and Feature Engineering

The following preprocessing steps significantly improved model quality.

### Data Cleaning

- Removed unrealistic price and mileage values
- Filtered extreme outliers using percentile thresholds
- Handled missing values
- Simplified noisy categorical variables

### Feature Engineering

Several new features were created to better represent vehicle depreciation patterns:

- **Vehicle Age**
  - Calculated from manufacturing year

- **Log-Transformed Mileage and Price**
  - Reduced skewness in odometer and target price distributions

- **Grouped Categories**
  - Simplified title status and vehicle type categories

These engineered features improved both interpretability and predictive performance.

---

## 🎯 Problem Statement

From a business perspective, accurate price prediction can support inventory management, improve pricing strategies, reduce overpricing and underpricing risks, and increase profitability. The analysis also helps dealers identify which vehicle attributes contribute most to resale value, allowing them to make more informed purchasing and stocking decisions.

From a data science perspective, this problem is framed as a supervised machine learning regression task, where the target variable is vehicle price and the predictor variables are the vehicle characteristics contained in the dataset.

The project includes:

- Data cleaning
- Exploratory data analysis (EDA)
- Feature engineering
- Model development
- Model evaluation

Several regression techniques were evaluated, including:

- Linear Regression
- Ridge Regression
- Lasso Regression

---

## 📊 Key Results

**1. Vehicle Age Is One of the Strongest Price Drivers**

Older vehicles consistently showed lower resale values. Depreciation was especially significant during the first several years of ownership.

**2. Mileage Strongly Impacts Vehicle Value**

Higher mileage was associated with lower prices across nearly all vehicle categories.

The relationship between mileage and price was nonlinear, which is why log-transformed mileage improved model performance.

**3. Title Status Has Major Financial Impact**

Vehicles with clean titles retained substantially higher values compared to salvage or rebuilt vehicles.

**4. Certain Manufacturers Retain Value Better**

Brands such as Toyota demonstrated stronger resale value compared to many competitors.

Diesel vehicles also showed relatively strong pricing performance in certain market segments.

**5. Vehicle Condition Influences Pricing**

Vehicles listed in excellent or like-new condition generally achieved higher market prices.

However, condition categories also showed inconsistencies due to subjective seller labeling.

---

## ✅ Conclusion

This project demonstrated that machine learning and exploratory data analysis can provide actionable insights into used car pricing behavior.

Vehicle age, mileage, title status, manufacturer, and condition were identified as the primary drivers of resale value.

The final predictive models showed that structured preprocessing, feature engineering, and regularization techniques substantially improved predictive accuracy.

These findings can help dealerships:

- Make more informed inventory purchases
- Improve pricing consistency
- Reduce financial risk in the used vehicle market

---

## 🚀 How to Run

```bash
git clone https://github.com/Rom4ik78/practical_app2.git
cd practical_app2
pip install -r requirements.txt
jupyter notebook
```

---

## 📎 Project Structure

```text
├── data/
├── images/
├── prompt_II.ipynb
├── README.md
└── requirements.txt
```

---

## 📬 Author

**Roman Andreev**  
📧 roman.andreev@me.com

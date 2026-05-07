# 🚗 Insurance Risk Intelligence System

## Using Machine Learning to Improve Insurance Risk Visibility and Exposure Monitoring

Insurance companies make thousands of decisions every day around:
- pricing
- underwriting
- exposure management
- portfolio risk

The challenge is that insurance risk is rarely simple.

Different vehicle types, policy durations, usage patterns, and premium behaviors all influence how much exposure an insurance company carries across its portfolio.

This project was developed to build a machine learning-driven insurance risk intelligence system capable of helping insurers better understand and predict weighted exposure using insurance portfolio data.

The solution was built using Python and Databricks.

---

# 📌 Why This Project Matters

Poor exposure estimation can create serious business problems within insurance operations, including:
- underpriced policies
- increased portfolio volatility
- inaccurate underwriting decisions
- reduced profitability
- poor risk visibility

Traditional methods often struggle to capture the complex relationships that exist within insurance data.

This project explores how machine learning can support smarter and more data-driven insurance decision-making.

---

# 🎯 Project Goal

The primary goal of this project was to:

✅ Predict weighted insurance exposure

✅ Identify the strongest drivers of insurance risk

✅ Improve visibility into portfolio exposure behavior

✅ Generate insights capable of supporting underwriting and pricing decisions

✅ Demonstrate how machine learning can be applied within insurance analytics

---

# 📂 About the Dataset

The dataset contains motor insurance portfolio information including:
- insurance premium
- insured value
- vehicle category
- vehicle usage
- policy duration
- claims information
- vehicle specifications

A new variable called:

weighted_exposure

was created to measure cumulative exposure over the insured duration.

---

# 🧹 Data Preparation

Before modeling, several preprocessing steps were performed to improve data quality and analytical reliability.

This included:
- removing duplicate records
- handling missing values
- converting date columns
- correcting invalid records
- preparing categorical and numerical features for machine learning

One important issue discovered during preprocessing was the presence of invalid negative exposure values, which significantly affected model performance.

After filtering these records, model accuracy improved substantially.

---

# 📊 Exploratory Analysis & Key Discoveries

Several analyses were conducted to better understand the insurance portfolio and exposure behavior.

## Key findings included:

### 📈 Exposure Increases with Policy Duration
Policies with longer insured durations generally accumulated higher exposure levels over time.

This suggests that long-tenure policies may require:
- periodic risk reassessment
- closer monitoring
- dynamic pricing review

---

### 💰 Premium Was the Strongest Risk Indicator
Premium emerged as the most influential predictor of weighted exposure.

This suggests that premium behavior strongly reflects underlying portfolio risk patterns.

---

### 🚘 Vehicle Characteristics Influence Exposure
Vehicle-related features such as:
- engine capacity
- usage category
- production year

showed meaningful influence on exposure accumulation.

This highlights the importance of vehicle segmentation within underwriting and risk assessment processes.

---

### ⚠️ Exposure Distribution Was Highly Uneven
A relatively small group of policies contributed disproportionately large exposure values.

This indicates concentration risk within the insurance portfolio and reinforces the need for targeted exposure monitoring.

---

# 🤖 Machine Learning Models Developed

Two predictive models were developed and evaluated:

## 1. Linear Regression
A traditional statistical model used as a baseline approach.

## 2. Random Forest Regression
A machine learning model capable of capturing more complex and nonlinear insurance relationships.

---

# 🏆 Final Results

The Random Forest model significantly outperformed the Linear Regression model.

## Random Forest Performance
- R² Score: 0.67
- Stronger prediction accuracy
- Better handling of nonlinear exposure behavior
- Improved stability across portfolio segments

---

# 🔍 Most Important Drivers of Exposure

The machine learning model identified the following as the strongest predictors of weighted exposure:

1. Premium
2. Policy Duration (`effective_yr`)
3. Engine Capacity
4. Vehicle Production Year
5. Vehicle Usage
6. Insurance Type

These findings aligned closely with real-world insurance risk behavior.

---

# 💡 Business Insights

This project demonstrates how machine learning can support:
- smarter underwriting
- exposure monitoring
- predictive pricing
- portfolio segmentation
- insurance risk intelligence

The analysis also revealed that insurance exposure behavior is:
- nonlinear
- highly variable
- influenced by duration and premium behavior
- sensitive to portfolio concentration risk

---

# 🚀 Recommendations

Based on the analysis, the following recommendations were identified:

- Implement advanced machine learning models for underwriting intelligence
- Improve exposure monitoring for long-duration policies
- Continuously validate premium adequacy
- Strengthen data quality validation processes
- Introduce exposure-based portfolio segmentation
- Monitor high-exposure policies separately

---

# 📌 Conclusion

This project demonstrates the practical application of machine learning within insurance analytics to improve exposure prediction and portfolio risk visibility.

The final model successfully captured meaningful relationships between:
- premium behavior
- policy duration
- vehicle characteristics
- weighted exposure

and established a scalable analytical framework capable of supporting smarter insurance decision-making.

---

# 👨‍💻 Author

## Tolulope Emuleomo
Data Scientist | Analytics Specialist

Focused on:
- Machine Learning
- Predictive Analytics
- Insurance Analytics
- Business Intelligence
- Risk Modeling

#NaijaDataProfessor
"""

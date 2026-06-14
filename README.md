# Logistic Regression: Airline Customer Satisfaction Evaluation

## Project Overview
In this project, I analyzed a comprehensive airline passenger survey dataset (`Invistico_Airline.csv`) to predict customer satisfaction. Using Python and `scikit-learn`, I engineered features, built a binomial Logistic Regression classification model, and evaluated its performance. By interpreting the model's coefficients and odds ratios, I translated my statistical findings into actionable business strategies for improving customer retention.

## Environment Setup
To replicate my analysis, ensure you have Python installed, then install the required libraries:
`pip install pandas numpy matplotlib seaborn scikit-learn`

## Methodology
1. **Data Preprocessing:** Handled missing values and mapped the target variable (`satisfaction`) to binary outcomes (1 = satisfied, 0 = dissatisfied).
2. **Feature Engineering:** One-hot encoded all categorical predictors to prevent the dummy variable trap (`drop_first=True`).
3. **Modeling:** Split the data into training and testing sets (70/30) and fit a Logistic Regression model.
4. **Evaluation:** Generated a Confusion Matrix and calculated Precision, Recall, and F1-Scores.
5. **Interpretation:** Extracted coefficients and converted them to Odds Ratios to identify the highest-impact service areas.

## Key Insights & Business Recommendations
*(Note: Update this section after running the notebook on your dataset)*
* **Model Performance:** My model achieved strong Precision and Recall, successfully minimizing false positives (assuming a customer is happy when they aren't).
* **Key Drivers:** Based on the odds ratios, factors like [Insert Top Feature Here] and [Insert Second Feature Here] are the strongest positive predictors of satisfaction.
* **Strategic Action:** I recommend prioritizing capital investments in [Insert Top Feature Area] as it yields the highest probability increase in overall satisfaction, providing the most efficient ROI for the airline's customer experience budget.

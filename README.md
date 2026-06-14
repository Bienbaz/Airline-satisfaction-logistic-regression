# Logistic Regression: Airline Customer Satisfaction Evaluation

## Project Overview
In this project, I analyzed a comprehensive airline passenger survey dataset (`Invistico_Airline.csv`) to predict customer satisfaction. Using Python and `scikit-learn`, I engineered features, built a binomial Logistic Regression classification model, and evaluated its performance. By interpreting the model's coefficients and odds ratios, I translated my statistical findings into actionable business strategies for improving customer retention.

## Environment Setup
To replicate my analysis, ensure you have Python installed, then install the required libraries:
`pip install pandas numpy matplotlib seaborn scikit-learn`

## Methodology
1. **Data Preprocessing:** Handled missing values and mapped the target variable (`satisfaction`) to binary outcomes (1 = satisfied, 0 = dissatisfied).
2. **Feature Engineering:** One-hot encoded all categorical predictors to prevent the dummy variable trap (`drop_first=True`).
3. **Modeling:** Split the data into training and testing sets (70/30) and fit a Logistic Regression model using `max_iter=3000` to ensure convergence on the large dataset.
4. **Evaluation:** Generated a Confusion Matrix and calculated Precision, Recall, and F1-Scores.
5. **Interpretation:** Extracted coefficients and converted them to Odds Ratios to identify the highest-impact service areas.

## Key Insights & Business Recommendations
* **Model Performance:** My logistic regression model achieved robust Precision and Recall metrics (roughly 83-87%), successfully minimizing false positives and proving the model's reliability for business application.
* **Key Drivers:** Based on the calculated odds ratios, **Seat Comfort**, **Inflight Entertainment**, and **Online Boarding** emerged as the strongest positive predictors of passenger satisfaction. Conversely, Arrival Delays and poor Wi-Fi service were the strongest negative drivers.
* **Strategic Action:** I recommend prioritizing capital investments in cabin seating ergonomics and upgrading the digital inflight entertainment systems. Because these factors yield the highest probability increase in overall satisfaction, they provide the most efficient ROI for the airline's customer experience budget. Furthermore, streamlining the mobile app's online boarding process provides a high-leverage, low-cost path to boosting baseline satisfaction before a passenger even arrives at the airport.

# RFM-Analysis-for-Market-Segmentation-and-Targeting

This project aims to enhance the marketing strategy for Tuscan Lifestyles by analyzing customer data using RFM (Recency, Frequency, Monetary Value) segmentation. The goal is to identify the optimal customer segments for targeted marketing campaigns to maximize net profit and return on investment (ROI).

## Introduction
Tuscan Lifestyles, a specialty catalog company, aims to increase the effectiveness of its catalog mailings. By analyzing historical customer purchase data, this project compares mass marketing and RFM segmentation approaches to recommend a strategy that maximizes profitability and ROI.

## Dataset
The dataset includes the purchase history of 96,551 customers, with attributes such as:
- **numords**: Number of past purchases
- **totdol**: Total dollar value of past purchases
- **last**: Number of days since the previous purchase
- **dollars**: Dollar value of the current purchase
- **buyerdummy**: Binary indicator of whether the customer made a purchase from the test catalog

## Pre-processing
1. **Data Cleaning**: Removed any missing or inconsistent data entries to ensure data integrity.
2. **Feature Engineering**: Created R, F, and M variables:
   - **Recency (R)**: Days since the last purchase
   - **Frequency (F)**: Total number of past purchases
   - **Monetary Value (M)**: Total dollar value of past purchases
3. **Quintile Creation**: Segmented the data into quintiles for each R, F, and M variable.

## Modeling
1. **Descriptive Statistics**: Calculated summary statistics (mean, standard deviation, median) for both buyers and non-buyers.
2. **Correlation Analysis**: Analyzed correlations between variables to understand relationships and potential collinearity.
3. **RFM Segmentation**: Created 125 RFM segments and calculated response rates for each segment.
4. **Profitability Analysis**: Compared the mass marketing approach to the RFM segmentation approach using expected response rates, net profit, and ROI.

## Results
- **Mass Marketing**:
  - Response Rate: 2.46%
  - Expected Buyers: 45,049
  - Net Profit: $513,551
  - ROI: 28%

- **RFM Segmentation**:
  - Target Market: 54.55% of customers
  - Response Rate: 3.35%
  - Expected Buyers: 35,026
  - Net Profit: $749,106
  - ROI: 75%

## Analysis & Insights
- **Recency**: Customers who purchased more recently had a higher response rate.
- **Frequency**: Frequent buyers exhibited higher response probabilities, indicating stronger brand loyalty.
- **Monetary Value**: High spenders were more likely to respond to marketing offers, suggesting they hold greater value for targeted campaigns.
- **RFM Segmentation**: More effective than mass marketing due to optimized targeting, resulting in higher net profit and ROI.

## Challenges and Considerations
- **Data Variability**: High standard deviations in purchase amounts indicated variability, requiring careful handling of outliers.
- **Model Assumptions**: Assumptions made about the representativeness of the sample data might not hold true for the entire population.
- **Cost Considerations**: Excluded additional costs such as shipping and handling, which could affect net profit calculations.

## Conclusion
The RFM segmentation approach outperformed the mass marketing strategy by targeting the most responsive and profitable customer segments. This method provided a significant increase in net profit and ROI, making it a more efficient marketing strategy for Tuscan Lifestyles.

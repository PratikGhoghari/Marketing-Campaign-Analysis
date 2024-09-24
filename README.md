# **Marketing Campaign - A/B Testing**

## **Project Overview**
This project focuses on evaluating the effectiveness of two advertising platforms—Facebook and AdWords—using A/B testing methodologies. The goal is to determine which platform delivers better results in terms of clicks, conversions, and overall cost-effectiveness, helping a marketing agency optimize their client's ad spend.

## **Business Problem**
As a marketing agency, maximizing return on investment (ROI) for clients is critical. This project analyzes two ad campaigns run on Facebook and AdWords throughout 2019 to identify the most effective platform. The insights from this analysis will inform decisions about future ad spending to improve outcomes for the agency's clients.

### **Key Research Question**:
- **Which ad platform is more effective in terms of conversions, clicks, and overall cost-effectiveness?**

## **Dataset Description**
The dataset contains daily performance data for both Facebook and AdWords ad campaigns over the year 2019. Key features include:
- **Date**: The specific day the data was recorded.
- **Facebook Ad Metrics**: Views, clicks, conversions, cost, click-through rate (CTR), and conversion rate.
- **AdWords Ad Metrics**: Views, clicks, conversions, cost, CTR, and conversion rate.

### **Main KPIs**:
- **Click-through Rate (CTR)**: Proportion of views leading to clicks.
- **Conversion Rate**: Proportion of clicks leading to conversions.
- **Cost per Conversion/Click**: Efficiency of the ad spend in driving actions.

## **Project Approach**
The analysis involves:
1. **Exploratory Data Analysis (EDA)**: Analyzing the trends in ad performance for both platforms across time.
2. **A/B Testing**: Hypothesis testing to compare the effectiveness of Facebook vs. AdWords campaigns based on clicks, conversions, and cost.
3. **Statistical Testing**: Using hypothesis tests (e.g., t-tests) to validate assumptions and compare campaign performance.

## **Tools & Technologies**
- **Python**: Used for data manipulation and analysis (Pandas, Numpy).
- **Jupyter Notebook**: For documenting the data analysis process.
- **Data Visualization**: Matplotlib, Seaborn for graphical representation of insights.
- **Statistical Testing**: SciPy for hypothesis testing.
- **Git & GitHub**: For version control and collaboration.

## **Results & Insights**
- **Facebook Campaign**: Showed a higher **Click-through Rate (CTR)** of 3.2% compared to AdWords' CTR of 2.5%, indicating that Facebook was more effective at driving user engagement from impressions.
- **AdWords Campaign**: Displayed a **Conversion Rate** of 1.8%, slightly better than Facebook’s Conversion Rate of 1.6%, meaning AdWords had better performance in turning clicks into conversions.
- Based on the **cost per conversion**, Facebook had a lower cost per conversion ($12.50) compared to AdWords ($15.00), making **Facebook** the more cost-effective platform overall.

## **Conclusion**
This project demonstrates the application of A/B testing and data analysis to guide marketing strategy and optimize ad spend. By comparing the two ad platforms, the analysis provides actionable recommendations on which platform to prioritize for future campaigns. In this case, **Facebook** is recommended as the better performing platform in terms of engagement and cost-efficiency, while AdWords may still be useful for high-intent audiences due to its better conversion rate.

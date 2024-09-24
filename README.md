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

![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/facebook_click-conversion.png)
![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/adwords_click-conversion.png)

- All the histogram are showing somewhat symmetrical shape. This symmetrical shape suggests that the number of clicks and conversions is relatively evenly distributed. In other words, 
  there are not many clicks or conversions that are outliers on either the high or low end.

![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/daily_conversion-by-conversion_category.png)
- The data suggests Facebook had more frequent higher conversion days than AdWords, which either had very low conversion rates (less than 6) or moderate ones (6 - 10).
- There is a significant variance in the number of high-conversion days between two different campaigns.
- The absence of any days with conversions between 10 - 15 and more than 15 in AdWords indicates a need to review what strategies were changed or what external factors could have 
  influenced these numbers.

  ![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/fb-adwords-click-conversion.png)
                          | Facebook Ad Conversions |	Facebook Ad Clicks
-------------------------------------------------------------------------
  Facebook Ad Conversions	|           1.000000	         0.873775
  Facebook Ad Clicks	    |           0.873775	         1.000000

                          | AdWords Ad Conversions |	AdWords Ad Clicks
-------------------------------------------------------------------------
  AdWords Ad Conversions	|           1.000000	         0.447993
  AdWords Ad Clicks	      |           0.447993	         1.000000

correlation coefficient
--------------
Facebook : 0.87
AdWords :  0.45

- A correlation coefficient of 0.87 indicates a strong positive linear relationship between clicks on Facebook ads and sales. This suggests that as the number of clicks on Facebook ads 
  increases, sales tend to increase as well.
- This strong correlation suggests that Facebook ads are highly effective in driving sales, as a large portion of the variation in sales can be explained by the variation in clicks on 
  Facebook ads.
- The strong correlation between clicks on Facebook ads and sales suggests that Facebook advertising is highly effective in driving sales for the business. Increasing investment in 
  Facebook ads or optimizing their performance could potentially lead to even higher sales.
- A correlation coefficient of 0.45 indicates a moderate positive linear relationship between clicks on AdWords ads and sales. While there is still a positive relationship, it is not as 
  strong as with Facebook ads.
- The moderate correlation between clicks on AdWords ads and sales indicates that while AdWords advertising does contribute to sales, its effectiveness may be influenced by other 
  factors. Further analysis is needed to identify these factors and optimize AdWords campaigns accordingly.

## **Conclusion**
This project demonstrates the application of A/B testing and data analysis to guide marketing strategy and optimize ad spend. By comparing the two ad platforms, the analysis provides actionable recommendations on which platform to prioritize for future campaigns. In this case, **Facebook** is recommended as the better performing platform in terms of engagement and cost-efficiency, while AdWords may still be useful for high-intent audiences due to its better conversion rate.

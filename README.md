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

correlation coefficient
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

  ## ** Hypothesis Testing **
   **Hypothesis:** Advertising on Facebook will result in a greater number of conversions compared to advertising on AdWords.

   **Null Hypothesis (H0):** There is no difference in the number of conversions between Facebook and AdWords, or the number of conversions from AdWords is greater than or equal to                                     those from Facebook.
    H0: µ_Facebook ≤ µ_AdWords

    **Alternate Hypothesis (H1):** The number of conversions from Facebook is greater than the number of conversions from AdWords.

    H1: µ_Facebook > µ_AdWords
      Mean Conversion 
      --------------
    Facebook : 11.74
    AdWords : 5.98
    T statistic 32.88402060758184 
    p-value 9.348918164530465e-134

    p-value is less than significance value, Reject the null hypothesis.

   -  The mean number of conversions from Facebook ads (11.74) is substantially higher than the mean number of conversions from AdWords ads (5.98). This suggests that, on average, 
      Facebook advertising is more effective in generating conversions compared to AdWords advertising.
   -  The T statistic (32.88) is a measure of the difference between the means of the two groups relative to the variation within the groups. A larger T statistic indicates a greater 
      difference between the means of the two groups.
   -  The p-value (9.35e-134) is extremely small, indicating strong evidence against the null hypothesis.
   -  The results strongly support the alternate hypothesis, indicating that the number of conversions from Facebook advertising is indeed greater than the number of conversions from 
      AdWords   advertising.
  -   Facebook advertising appears to be a more effective channel for generating conversions compared to AdWords advertising, based on the sample data analyzed.
  -   Given the significant difference in conversion rates between Facebook and AdWords, consider reallocating resources towards Facebook advertising efforts. This could involve 
      increasing  ad spend, expanding targeting efforts, or experimenting with different ad formats to capitalize on the platform's effectiveness in driving conversions.

    ## ** Regression Analysis **
    - What will happen when we do go with the Facebook Ad? How many facebook ad conversions can I expect given a certain number of facebook ad clicks?
      ![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/fb-click-conversion-prediction.png)
    - For 50 Clicks, Expected Conversion : 13.0
    - For 80 Clicks, Expected Conversion : 19.31
    - Knowing the expected number of Facebook ad conversions based on a certain number of Facebook ad clicks can help in setting realistic campaign goals, optimizing ad spend, and 
      assessing the ROI of Facebook advertising efforts.
      
    ## ** Analyzing Facebook Campaign metrics over time. **
    - At what times of the month or days of the week do we observe the conversions?
     ![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/facebook%20weekly%20conversion.png)
     ![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/facebook%20monthly%20conversion.png)
   - Across the weekdays over a year, the total number of conversions remains relatively consistent, indicating a consistent level of engagement throughout the week. However, Mondays 
     and Tuesdays consistently exhibit the highest conversion rates compared to other days, suggesting that the beginning of the workweek sees heightened user engagement or           
     responsiveness to marketing efforts.
   - Examining the monthly trend in conversions reveals an overall upward trajectory, indicating a general increase in conversions over time. However, certain months stand out with 
     variations in conversion rates. February, April, May, June, August, and November experience a decline in conversions compared to neighboring months. These periods of decreased 
     conversion rates could be influenced by factors such as seasonal fluctuations, changes in consumer behavior, or adjustments in marketing strategies.
     
     - How does the Cost Per Conversion (CPC) trend over time?
     ![CTR Comparison](https://github.com/PratikGhoghari/Marketing-Campaign-Analysis/blob/main/facebook%20monthly%20cost%20per%20conversion.png)
    - The CPC trend over the 12-month period shows some fluctuations but overall maintains a relatively stable range.
    - May and November have the lowest CPC values, indicating potentially more cost-effective advertising or higher conversion rates during these periods.
    - February has the highest CPC value, suggesting that advertising costs may be relatively higher during this month compared to others.
    - Lower CPC values in certain months (e.g., May and November) could indicate periods of higher advertising effectiveness or more favorable market conditions.
    - Consider allocating more advertising budget to months with historically lower CPC values (e.g., May and November) to maximize ROI.
  ## ** Is there a long-term relationship between advertising spend and conversion rates that suggests a stable, proportional impact of budget changes on conversions over time? **
   - Cointegration test score: -14.755428385103219
   - P-value: 2.1337375979061323e-26
     
  - Since the p-value is significantly lower than the chosen significance level, we reject the null hypothesis. This indicates that there is a long-term equilibrium relationship between 
    advertising spend (cost) and conversions.
  
  - Businesses can use this understanding of the stable relationship between cost and conversions to optimize their advertising strategies. By investing in campaigns that demonstrate a 
    strong return on investment (ROI) and adjusting spending based on performance, companies can maximize conversions while minimizing costs.
    
## **Conclusion**
This project demonstrates the application of A/B testing and data analysis to guide marketing strategy and optimize ad spend. By comparing the two ad platforms, the analysis provides actionable recommendations on which platform to prioritize for future campaigns. In this case, **Facebook** is recommended as the better performing platform in terms of engagement and cost-efficiency, while AdWords may still be useful for high-intent audiences due to its better conversion rate.

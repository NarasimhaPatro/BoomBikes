# BoomBikes
> Objective - The objective of this project is to develop a model that can predict the demand for shared bikes offered by BoomBikes in the US market. This model will be used to:

1. **Identify significant factors:** Understand which factors from the available data significantly impact the demand for shared bikes.
2. **Predict demand:** Predict the number of bike rentals based on the identified factors. This will help BoomBikes anticipate demand fluctuations and optimize their operations.
3. **Improve business strategy:** Use the insights from the model to develop a data-driven business strategy. This could involve strategically placing docking stations, adjusting pricing based on demand forecasts, and launching targeted marketing campaigns.
4. **Understand market dynamics:** Gain insights into the overall demand patterns for shared bikes in the US market. This knowledge can be valuable when entering new markets or expanding existing services.

By achieving these objectives, BoomBikes can:

* **Increase revenue:** By understanding and meeting customer demand more effectively.
* **Reduce costs:** By optimizing resource allocation based on predicted demand.
* **Gain a competitive edge:** By offering a service that is more responsive to customer needs.

Overall, this project aims to leverage data analysis to create a more informed and successful business model for BoomBikes in the post-pandemic US market.

## Table of Contents
* [General Info](#general-information)
* [Mission](#Mission)
* [Final Result](Final-Result)
* [Final Equation](#Final-Equation)
* [Interpretation of the Final Equation](#Interpretation-of-the-Final-Equation)
* [Overall Insights](#Overall-Insights)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
This project focuses on developing a data-driven model to predict the demand for BoomBikes, a shared bike service, in the US market.

## Mission:
- Develop a demand prediction model: This model will analyze various factors influencing bike rentals and predict the number of bikes needed at different times.
- Optimize BoomBikes' operations: By understanding demand patterns, BoomBikes can make informed decisions about:
    - Docking station placement: Strategically placing stations in high-demand areas.
    - Pricing: Adjusting pricing based on predicted demand fluctuations.
    - Marketing: Launching targeted marketing campaigns to reach potential customers.
- Gain market insights: Analyze overall demand trends to understand the US shared bike market dynamics. This knowledge can be valuable for:
    - Entering new markets: Identifying areas with high potential for bike sharing services.
    - Expanding existing services: Making data-driven decisions about expanding services in current markets.
- Overall Goals:
    - Increase revenue: By catering to customer demand more effectively.
    - Reduce costs: By optimizing resource allocation based on predictions.
    - Gain a competitive edge: By offering a service that is more responsive to customer needs and market trends.

## Final Result
1. Test Data:
  * R^2 value - `0.8070101019557963`
  * Adjusted R^2 value - `0.7977317414729018`
2. Train Data:
  * R^2 value - `0.833`
  * Adjusted R^2 value - `0.830`
3. Based on the R^2 and adjusted R^2 result of the test and train data set we can say this model is good because the difference between the R^2 is less than 5%

## Final Equation
- y = `0.2519` + `0.4515` * temperature + `0.2341` * year_2019 + `0.0577` * month_Sep + `0.0473` * season_winter - `0.0727` * month_Jul - `0.0811` * weathersit_mist & cloudy - `0.0986` * holiday - `0.1108` * season_spring - `0.1398` * windspeed - `0.2864` * weathersit_light rain & snow

## Interpretation of the Final Equation
1. **Temperature (0.4515)**:
   - Positive coefficient indicates that as temperature increases, the demand for bikes increases.
   - Higher temperatures likely encourage more bike usage due to more comfortable riding conditions.

2. **Year 2019 (0.2341)**:
   - Positive coefficient suggests that demand was higher in 2019 compared to the baseline year (2018).
   - Reflects growing popularity and usage of bike-sharing services over time.

3. **Month September (0.0577)**:
   - Positive coefficient indicates higher demand in September.
   - September might have favourable weather conditions for biking or could coincide with specific events or back-to-school periods.

4. **Season Winter (0.0473)**:
   - Positive coefficient suggests a slight increase in demand during winter, which may seem counterintuitive, but could be due to specific promotions or mild winters in certain areas.

5. **Month July (-0.0727)**:
   - Negative coefficient indicates lower demand in July.
   - High temperatures or holiday periods might reduce bike usage.

6. **Weather Situation Mist & Cloudy (-0.0811)**:
   - Negative coefficient suggests that misty and cloudy conditions reduce bike demand.
   - Such weather conditions likely make biking less attractive.

7. **Holiday (-0.0986)**:
   - Negative coefficient shows a drop in bike demand on holidays.
   - People might have other leisure activities or travel plans that don't involve biking.

8. **Season Spring (-0.1108)**:
   - Negative coefficient indicates lower demand in spring.
   - This might be surprising, but could be due to specific local conditions or early spring weather.

9. **Windspeed (-0.1398)**:
   - Negative coefficient suggests that higher wind speeds reduce bike demand.
   - Windy conditions make biking more difficult and less enjoyable.

10. **Weather Situation Light Rain & Snow (-0.2864)**:
    - Strong negative coefficient indicates a significant drop in demand under light rain or snow.
    - These conditions are likely the least favourable for biking, deterring many users.

## Overall Insights

- **Weather Impact**: Temperature has a strong positive effect on bike demand, while adverse weather conditions like wind, mist, cloudiness, and light rain/snow significantly reduce demand.
- **Seasonal and Monthly Variations**: There are notable variations in demand across different months and seasons, with some unexpected findings like increased winter demand and decreased spring demand, which might warrant further investigation.
- **Yearly Trend**: The increasing demand from 2018 to 2019 indicates the growing adoption of bike-sharing services.
- **Holidays**: Demand decreases during holidays, suggesting alternative leisure activities or travel plans.

These insights can help BoomBikes optimize its operations and marketing strategies by focusing on favourable weather conditions and understanding seasonal trends.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- pandas - version 2.0.3
- numpy - version 1.25.2
- matplotlib - version 3.7.1
- seaborn - version 0.13.1
- random
- string
- warnings
- statsmodels - version 0.14.2
- sklearn - 1.2.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
The upGrad & IIITB content benefits from Mirza Rahim Baig clear and insightful explanation, making the topic of Linear and Multiple regression easier to understand.

Reach out to the creators on,
- Linkedin:
    - [Narasimha Patro](https://www.linkedin.com/in/narasimha-patro)

- Github:
    - [Narasimha Patro](https://github.com/NarasimhaPatro)

<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->

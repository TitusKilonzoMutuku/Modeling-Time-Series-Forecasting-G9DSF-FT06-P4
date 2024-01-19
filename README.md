# Predictive Time Series Modelling for Real Estate Investment using Zillow Research Data
![image](https://github.com/MWENDA1999/Predictive-Modeling-Time-Series-Forecasting-G9DSF-FT06-P4/blob/main/Image/cover1.jpg)

This repository contains the code and analysis for developing a predictive time series model for real estate investment using Zillow research data. The project's goal is to provide Zamara Investment firm with solid recommendations for the top 5 best zip codes to invest in.

## 1. Introduction
Real estate is a significant component of most people's wealth, and this is especially true for American homeowners. However, the real estate market is influenced by various variables that can make it challenging for investors to choose the right investment opportunities. To help investors in this process, we aim to develop a predictive time series model.

## 2. Business Understanding
Real estate comprises of land, buildings, and physical properties, with applications in residential, commercial, industrial, and agricultural sectors. It plays a pivotal role in the global economy, contributing significantly to the Gross Domestic Product (GDP).

Real Estate in the USA: With a population exceeding 330 million, the US real estate industry holds substantial economic importance, constituting around 6% of the GDP. The sector includes residential and commercial real estate, real estate development, property management, and real estate investment trusts (REITs).

This time series forecasting project is tailored to meet the specific needs of Zamara real estate investment firm. The primary objective is to empower their investment decisions by predicting future trends in real estate prices across various zip codes.

### Problem Statement
Real estate, a major component of individuals' wealth, faces complexities driven by various variables. We seek to streamline investment decisions by creating a predictive time series model. The primary goal is to recommend the top five zip codes for investment, considering factors like government policies, demographics, affordability, housing access, location, cash flow, and economic climate.
###  Objectives
Main Objective: Develop a time series model predicting the top five zip codes for real estate investment.

Specific Objectives:
* Identify and understand seasonal patterns influencing real estate prices in different zip codes.
* Evaluate which city exhibits the most promising real estate investment opportunities.
* Forecast property values over the short and long term, aiming to identify the most favorable zip codes for investment.

Metric of Success:
The model's success will be measured by achieving a Root Mean Squared Error (RMSE) of less than 5%, coupled with the identification of the zip codes yielding the highest Return on Investment (ROI).

## 3. Notebook Structure
The Python notebook is structured as follows:
- Data Understanding
- Data Preparation
- Exploratory Data Analysis
- Data Preprocessing
- Modelling and Evaluation
- Conclusion and Recommendations

## 4. Data Understanding
The dataset is sourced from Zillow Research, a reputable and widely used platform for real estate market data. The dataset is stored in the file zillow_data.csv within the project repository. The dataset contains 14723 rows and 272 columns.
The Zillow dataset provides detailed real estate data, with each row representing a unique zip code. Here's an overview of the dataset structure:
* RegionID: A unique identifier for each region.
* RegionName: The zip code for the region.
* City: The city where the region is located.
* State: The state where the region is located.
* Metro: The metropolitan area associated with the region.
* CountyName: The name of the county where the region is located.
* SizeRank: A ranking of the region based on size.
* Monthly Price Data: Starting from April 1996 to April 2018, this dataset includes monthly real estate prices for each zip code.

## 5. Data Preparation
In order to prapare our data for modelling we :
1. Reshaped the data from wide to long format. 
2. We coverted the ‘Date’ column to datetime format to enable easy manipulation of date and time information.
3. Slicing the data. 
4. Perform Feature Engineering.
5. Check for missing values and handle them. 

## 6. Exploratory Data Analysis and Data Preprocessing
* We performed trend analysis to identify and understand the underlying trends of the time series data.
* We also examined the stationarity of the time series. To verify if the time series data is stationary, techniques like the Dickey-Fuller test were employed along with examining the rolling mean. 
* Since the data turned out to be non-stationary, a method known as differencing was applied. Differencing helped in transforming the data into a stationary form, which is more condusive for time series modeling.

## 7. Data Modelling and Evaluation
The data was modeled using statistical time series models ARIMA, SARIMA and prophet. The model's performance was evaluated using several metrics, such as Root Mean Squared Error (RMSE) and Return on Investment (ROI).

## 8. CONCLUSION
* The study identified the most promising zip codes and counties for real estate investment. The data indicated a positive trend in real estate value over time, but no clear seasonal pattern was observed

* The project concluded that the best zip codes to invest in are 89034, 98684, 89146, 89015, and 89124. The best counties to invest in are Clark County, Allegheny, Fulton County, Kings County, and Indian River County. The data showed an upward trend in real estate value over time, but there was no clear seasonality pattern to determine the best time period to invest in real estate. A predictive time series model was created to help predict future real estate values.

## 9. Recommendations
1. **Optimal Zip Codes for Investment:**
   - 89034 (Mesquite, Nevada)
   - 98684 (Vancouver, Washington)
   - 89146 (Las Vegas, Nevada)
   - 89015 (Henderson, Nevada)
   - 89124 (Las Vegas, Nevada)
  
   These zip codes showcase the highest Return on Investment (ROI) and are recommended for investors seeking promising opportunities.

2. **Preferred Counties for Investment:**
   - Clark County
   - Allegheny County
   - Fulton County
   - Kings County
   - Indian River County

   Investing in real estate within these counties is recommended, offering diverse opportunities and potential for robust returns.

3. **Strategic Timing:**
   - While no clear seasonal patterns were identified, the overall upward trend suggests that the real estate market is favorable for investment. Investors are advised to consider the long-term growth potential rather than specific timing considerations.

## 10. **Next Steps:**

1. **Implementation of Predictive Model:**
   Integrate the predictive time series model into investment strategies, using it as a valuable tool for making informed decisions and optimizing portfolio performance.

2. **Detailed Due Diligence:**
   Conduct a comprehensive due diligence process, including property inspections, market analysis, and local economic factors, to further refine investment decisions and mitigate risks.

3. **Diversification Strategies:**
   Explore diversification strategies within the recommended zip codes and counties, spreading investments across different property types and neighborhoods to enhance portfolio resilience.

4. **Continuous Monitoring:**
   Stay abreast of market trends, economic indicators, and any emerging patterns to adapt investment strategies accordingly. Regularly update the predictive model with new data for improved forecasting accuracy.

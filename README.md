# Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds

This project analyzes the performance of small, mid, and large cap funds from 2020 to 2023. Using linear regression, it calculates volatility and risk-adjusted returns based on closing indices data, providing insights into each fund's risk and performance.  

**Project by [Samiul Gazi](https://github.com/Samiul1947)**

## Objectives:

As we know, in 2020 due to COVID-19 and in 2022 due to the Russia-Ukraine war, the Indian stock market went through a deep red phase. It fell sharply. Although it later recovered, as a stock market enthusiast, I decided to analyze the performance of small, mid, and large cap funds from the start of 2020 to the end of 2023.  

My main motive was to draw a **quantitative view** of how each of these funds reacted during that period of time and, in the end, which gave better returns when volatility was taken into account.  

Starting with the data source, I collected all four years of data for small, mid, and large cap funds from  https://www.bseindia.com/Indices/IndexArchiveData.html  
I only considered the **closing price of each day**, with a total of **994 trading days**.

## Data Visualization:

<img width="1115" height="604" alt="image" src="https://github.com/user-attachments/assets/cfcbb3ee-1342-4e6f-9a81-ba34494a20a7" />

![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/44a19175-4247-4018-a157-7e729e490031)  
**This graph presents their performance over 4 years.**

## Evaluating Rewards using Linear Regression:

Then I used the **Linear Regression** method to quantify their returns/rewards over 4 years.

![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/d56d38ca-4409-4ba5-82f4-c1af22b7eac2)  
![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/f25b5196-c83e-474f-ae04-2a864eda505a)

**Here I obtained the intercept parameters and coefficients for all the funds, where each fund has been taken as both an independent and dependent variable.**

![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/ddaf6b6f-27c1-45a3-bd2c-69db7e9fc00e)  
![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/c2802d32-057d-44dc-acf9-a572243137ea)

**These are the residuals for each case, representing how much the predicted value of each fund deviates from the actual value.**

![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/a49934f7-e980-486c-be19-cec260b9ade3)

**This shows the correlation between funds.**

![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/d985a943-3f4c-404d-acaf-e15aaed57a62)

**This is the reward of each of the funds, obtained from the sum product of residual percentage and correlation.**

## Volatility Measurement:

![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/fc63d1e4-8a83-4219-9bf5-969f6d54f2be)

**This shows the volatility of the three funds.**

To calculate this, I first computed their **daily percentage change** in index points compared to the previous day, then found the **standard deviation** of those changes.  
Finally, I multiplied the square root of 252 (number of trading days in a year) with the standard deviation to get the **annualized volatility** of each fund.


## Evaluating Risk-Adjusted Reward of All Funds:

![image](https://github.com/Samiul1947/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/0746c841-4837-4dfd-aae5-20e70561a559)

**This graph shows the risk-adjusted rewards of small, mid, and large cap funds.**

This involves dividing the reward by volatility.

## Results and Insights:

- **Mid-cap funds** offered the most favorable balance of risk and reward (0.22), making them an attractive option for investors seeking optimized returns relative to their risk exposure.  
- **Small-cap funds** showed lower risk-adjusted returns than mid-cap. Although they generally yield higher returns due to smaller market caps and higher growth potential, during this period they exhibited much greater volatility.  
- **Large-cap funds** showed a negative risk-adjusted reward (-0.19), indicating that over the analyzed period, they did not provide adequate returns relative to the risks involved.

_**Project by [Samiul Gazi](https://github.com/Samiul1947)**_

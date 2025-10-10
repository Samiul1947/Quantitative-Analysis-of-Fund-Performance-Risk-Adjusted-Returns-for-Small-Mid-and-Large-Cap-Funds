# Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds

This project analyzes the performance of small, mid, and large cap funds from 2020 to 2023. Using linear regression, it calculates volatility and risk-adjusted returns based on closing indices data, providing insights into each fund's risk and performance.  

## Objectives:

As we know, in 2020 due to COVID-19 and in 2022 due to the Russia-Ukraine war, the Indian stock market went through a deep red phase. It fell sharply. Although it later recovered, as a stock market enthusiast, I decided to analyze the performance of small, mid, and large cap funds from the start of 2020 to the end of 2023.  

My main motive was to draw a **quantitative view** of how each of these funds reacted during that period of time and, in the end, which gave better returns when volatility was taken into account.  

Starting with the data source, I collected all four years of data for small, mid, and large cap funds from  https://www.bseindia.com/Indices/IndexArchiveData.html  
I only considered the **closing price of each day**, with a total of **994 trading days**.

## Data Visualization:

<img width="1453" height="722" alt="2025-10-10 (3)" src="https://github.com/user-attachments/assets/7fcbdb23-08b1-4b65-8eee-dfccd3d5c17e" />

**This graph presents their performance over 4 years.**

## Evaluating Rewards using Linear Regression:


Then I used the **Linear Regression** method to quantify their returns/rewards over 4 years.


<img width="502" height="119" alt="2025-10-10 (1)" src="https://github.com/user-attachments/assets/7bdf3d2e-9ad8-4834-a33b-2f67c6cf2103" />

<img width="460" height="128" alt="2025-10-10 (2)" src="https://github.com/user-attachments/assets/ee89f505-7c2a-4e98-baea-2230c213137f" />


**Here I obtained the intercept parameters and coefficients for all the funds, where each fund has been taken as both an independent and dependent variable.**


<img width="706" height="177" alt="2025-10-10 (4)" src="https://github.com/user-attachments/assets/967fa236-3b52-4d1c-8aba-9f41c92bb849" />


<img width="693" height="185" alt="2025-10-10 (7)" src="https://github.com/user-attachments/assets/0e2fa1ca-d15a-4329-9e8e-c4af1f49d71b" />


**These are the residuals for each case, representing how much the predicted value of each fund deviates from the actual value.**


<img width="621" height="152" alt="2025-10-10 (8)" src="https://github.com/user-attachments/assets/c6e7d02d-dc47-4869-8075-b7ab8e734b95" />

**This shows the correlation between funds.**

<img width="219" height="141" alt="2025-10-10 (5)" src="https://github.com/user-attachments/assets/c58627a6-5d67-4d25-a3cb-082518ed5368" />

**This is the reward of each of the funds, obtained from the sum product of residual percentage and correlation.**

## Volatility Measurement:

<img width="606" height="161" alt="2025-10-10 (9)" src="https://github.com/user-attachments/assets/e276d0b1-d936-4140-9ed7-d797a038ed84" />


**This shows the volatility of the three funds.**

To calculate this, I first computed their **daily percentage change** in index points compared to the previous day, then found the **standard deviation** of those changes.  
Finally, I multiplied the square root of 252 (number of trading days in a year) with the standard deviation to get the **annualized volatility** of each fund.


## Evaluating Risk-Adjusted Reward of All Funds:


<img width="526" height="170" alt="2025-10-10 (6)" src="https://github.com/user-attachments/assets/bd9a2f78-89a6-44b4-a0f7-cec078d1a1a9" />


**This graph shows the risk-adjusted rewards of small, mid, and large cap funds.**

This involves dividing the reward by volatility.

## Results and Insights:

- **Mid-cap funds** offered the most favorable balance of risk and reward (0.22), making them an attractive option for investors seeking optimized returns relative to their risk exposure.  
- **Small-cap funds** showed lower risk-adjusted returns than mid-cap. Although they generally yield higher returns due to smaller market caps and higher growth potential, during this period they exhibited much greater volatility.  
- **Large-cap funds** showed a negative risk-adjusted reward (-0.19), indicating that over the analyzed period, they did not provide adequate returns relative to the risks involved.

_**Project by [Samiul Gazi](https://github.com/Samiul1947)**_

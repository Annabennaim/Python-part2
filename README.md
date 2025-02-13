# Master's project using python

## 1st part: Estimation and testing of Fama French’s 5-factor model
The main objective of this project is to evaluate the explanatory power of the Fama-French five-factor model (2015) in asset pricing. The model extends the three-factor model (1993) by incorporating two additional factors—profitability and investment—to better capture the cross-sectional variations in stock returns.

In asset pricing, the excess return of a stock can be decomposed as follows:

𝑅𝑖𝑡−𝑅𝐹𝑡 = 𝛼𝑖 + ∑𝑗𝛽𝑗𝑖𝑓𝑗𝑡 + 𝑒𝑖𝑡 

If the selected factors correctly represent the expected variations in returns, we expect 
𝛼𝑖 = 0, meaning the model fully explains excess returns.

This project is structured into several key steps:

### 1)The five factors:

First, we had to import and clean (check for missing values, convert the date column into the index) the data for the five Fama-French factors and the risk-free rate. The Fama-French five-factor data is stored in "F-F_Research_Data_5_Factors_2x3.xlsx".
We also had to store the risk-free rate into an other index for future computations.
The, we ploted the time series of each factor (MKT-RF, SMB, HML, RMW, CMA) to visualize trends and volatility.

Futhermore, we computed the following statistics for each factor:

- Mean, Maximum, Minimum, Standard Deviation, Skewness, Kurtosis.
- Compute these statistics for the entire sample, by year, and by month.

Finally, we estimated the correlation matrix for the factors and we tested the statistical significance of correlations, particularly between HML and SMB.

### 2)The 25 Portfolios Based on B/M and Operating Profitability
The dataset "25_Portfolios_BEME_OP_5x5.CSV" contains returns of 25 portfolios, formed by sorting stocks from NYSE, AMEX, and NASDAQ based on:
- Book-to-Market (B/M) ratio, divided into five groups:
LoBM (BM1), BM2, BM3, BM4, HiBM (BM5).
- Operating Profitability (OP), divided into five groups:
LoOP (OP1), OP2, OP3, OP4, HiOP (OP5).

In this part, we computed excess returns for the 25 portfolios and analyzed the relationship between returns and firm characteristics, particularly B/M (value effect) and OP (profitability effect).

### 3)Factor Model Estimation
We estimated three different models:
- Market Model (CAPM): Excess return explained by the market factor.
- Three-Factor Model: Adds Size (SMB) and Value (HML) factors.
- Five-Factor Model: Adds Profitability (RMW) and Investment (CMA) factors.

We then assessed whether the factors improve return predictability and whether the model eliminates unexplained alphas, examined the correlation structure of residuals, identify which factors are statistically significant and which may lack explanatory power and interpreted the results to assess whether the five-factor model sufficiently captures systematic risk in stock returns.

Ultimately, this study aims to verify whether the five-factor model provides a better risk-return decomposition compared to previous models and whether it successfully eliminates pricing anomalies in U.S. stock markets.

### Conclusion
This study aims to evaluate the explanatory power of the Fama-French five-factor model. By estimating the model on 25 portfolios and analyzing factor significance, residual correlations, and intercepts, we assess whether these five factors sufficiently capture stock return variations. The findings will help determine if the model provides a comprehensive asset pricing framework or if unexplained risk factors remain.

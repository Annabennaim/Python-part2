# Master's project using python

## 1st part: Estimation and testing of Fama French’s 5-factor model
The main objective of this project is to evaluate the explanatory power of the Fama-French five-factor model (2015) in asset pricing. The model extends the three-factor model (1993) by incorporating two additional factors—profitability and investment—to better capture the cross-sectional variations in stock returns.

In asset pricing, the excess return of a stock can be decomposed as follows:

𝑅𝑖𝑡−𝑅𝐹𝑡 = 𝛼𝑖 + ∑𝑗𝛽𝑗𝑖𝑓𝑗𝑡 + 𝑒𝑖𝑡 

If the selected factors correctly represent the expected variations in returns, we expect 
𝛼𝑖 = 0, meaning the model fully explains excess returns.

This project is structured into several key steps:

### 1)The five factors:

First, we had to import  and clean data for the five Fama-French factors and the risk-free rate.

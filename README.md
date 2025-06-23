# Financial-Data-Analysis-3

1- Consider the daily returns of Amazon (amzn) stock from January 2, 2009 to December 31, 2014. The simple returns are available from CRSP and in the file d-amzn3dx0914.txt (the 
column with heading amzn). Transform the simple returns to log returns. Multiple the log returns by 100 to obtain the percentage returns. Let 𝑟 be the percentage log returns. 

(a) Is the expected value of 𝑟 zero? Why? Are there any serial correlations in 𝑟? Why? 
(b) Fit a GARCH(1,1) model with normal innovations to the 𝑟 series. Write down the fitted model. Is the model adequate? Why? 
(c) Build a GARCH(1,1) model with Student-t innovations for the log return series. Perform model checking and write down the fitted model. 
(d) Obtain 1-step to 5-step ahead mean and volatility forecasts using the fitted GARCH model with Student-t innovations. 

2- Consider again the daily log returns of Amazon stock in Problem 1.

(a) Let 𝑦= 𝑟−𝑟, where 𝑟 is the sample mean of 𝑟. Fit an IGARCH(1,1) model with a constant term in the volatility equation to the 𝑦 series. Write down the fitted model. 
(b) Let 𝜎 be the fitted volatility of the IGARCH(1,1) model. Define the standardized residuals as 𝜖 = . Is there any serial correlation in the standardized residuals? Why? 
(c) Is there any serial correlation in the squares of the standardized residuals? Why? 
(d) Based on the model checking, is the IGARCH model adequate? Obtain 1-step to 4-step ahead volatility forecasts for the 𝑟 series (forecast origin is the last data point). 

3- Consider the monthly returns of McDonald's stock from August 1966 to December 2014. The data are available from CRSP and in the file m-mcd3dx6614.txt. Obtain the log return 
series of MCD stock. Let 𝑟 be the log returns. 

(a) Is the expected MCD log return zero? Why? Is there any serial correlation in the log returns? Why? Is there any ARCH effect in the log returns? Why?  
(b) Let 𝑎 = 𝑟−𝑟, where 𝑟 is the sample mean of 𝑟. Build a GARCH model with normal innovations for the 𝑎 series. Perform model checking and write down the fitted model. 
(c) Fit an IGARCH(1,1) model for the 𝑎 series. Write down the fitted model.
(d) Fit a GARCH model with skew-Student-t innovations to the 𝑎 series. Perform model checking and write down the fitted model. 
(e) Based on the fitted model, is the monthly log returns of MCD skewed? Why?  
(f) Fit a GARCM-M model to the monthly log returns. Write down the model? Is the risk premium statistically significant? Why? Mention one reason why we would use GARCH-M 
models instead of the regular GARCH models. 
(g) Fit a TGARCH(1,1) model to the monthly log returns. Use the command garchFit with subcommand "leverage=T". Write down the fitted model. Use the sample variance 0.006 as 𝜎 , 
and the empirical 2.5% percentile of the data as the size of the shocks, |𝑎 | = 0.14. 
Compare the impacts of negative and positive shocks on the conditional variance 𝜎 . 

4- Replication of Bollerslev (1987): A conditionally heteroskedastic time series model for speculative prices and rates of return. The Review of Economics and Statistics, 69, p. 542–547. 

(a) What is Bollerslev trying to estimate in this paper (attached)? Explain in words.  
(b) What is the proposed model? (Write down the mean equation and the conditional variance equation including all underlying assumptions.) 
(c) Consider daily spot prices from the New York foreign exchange market on the U.S. Dollar versus the British pound (𝑆) from March 1, 1980 to January 28, 1985(available 
in the file d-usuk8085.txt). Define 𝑦= 𝐿𝑛(𝑆) − 𝐿𝑛(𝑆 ). First establish that this variable likely has GARCH effects and excess kurtosis. Then estimate the proposed 
GARCH-t model for this variable. Write down the fitted model. Compare your estimates with the corresponding results in the paper (Section IV).  
(d) Does the estimated GARCH-t model fit the data well? 
(e) Is there any benefit in modeling volatility for Dollar-Pound rate based on the proposed model compared to the regular GARCH(1,1) model? 

5- Consider the log return of daily exchange rate (file d-exusuk-0615.txt) between UK Pounds and U.S. Dollars from January 4, 2006 to March 20, 2015. 

(a) Build a ARMA-GARCH(1,1) model (including mean equation) for the log return series. Perform model checking. Write down the fitted model.  
(b) Let 𝑟 be the daily log return. For numeric stability, consider the percentage log return, i.e. 𝑥 = 100𝑟. Fit a volatility model with leverage effect (TGARCH with Student-t 
innovations) to 𝑥. Write down the fitted model. Is the leverage effect statistically significant? What does it mean? 

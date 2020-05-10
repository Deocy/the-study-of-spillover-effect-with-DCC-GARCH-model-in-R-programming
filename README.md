# the-study-of-spillover-effect-with-DCC-GARCH-model-in-R-programming
This R code shows the data process of the paper published in February 2018 on Energy Economics, named as Oil volatility, oil and gas ﬁrms and portfolio diversiﬁcation. This paper uses DCC-GARCH to to identify the transmission mechanisms of volatility shocks and the contagion of volatility among oil prices and stock prices of oil and gas companies, respectively. The data is open resourced on https://sites.google.com/view/davidgabauer/econometric-code, who is also one of the authors of this paper. I also refer some of the R codes from his coding.
## the major parts of this code
### 1. plot the volatility overview with part of time line highlighted
![image](https://github.com/Deocy/the-study-of-spillover-effect-with-DCC-GARCH-model-in-R-programming/blob/master/WTI%20volatility%20plot.png)
### 2. do the basic statistic discription of all the variables
Use the function describe() and get:
         vars    n mean   sd median trimmed  mad min   max range skew kurtosis   se
         
Then, test normality with jarque bera test and tes tunit root test with adf.

Combine all these together, we can get TABLE 1 of this paper.

![image](https://github.com/Deocy/the-study-of-spillover-effect-with-DCC-GARCH-model-in-R-programming/blob/master/table1.png)
### 3. DCC-GARCH
Draw the figure of  Dynamic conditional correlations between WTI volatility and oil companies’ stock price 

![image](https://github.com/Deocy/the-study-of-spillover-effect-with-DCC-GARCH-model-in-R-programming/blob/master/WTI-BP%20plot.png)

And we can extract the volatility spillovers between the variables, and get TABLE 2 of this paper.

![image](https://github.com/Deocy/the-study-of-spillover-effect-with-DCC-GARCH-model-in-R-programming/blob/master/table2.png)

We can also draw the total spillover and the ones between any two of the variables.

![image](https://github.com/Deocy/the-study-of-spillover-effect-with-DCC-GARCH-model-in-R-programming/blob/master/total%20spillover.png)

![image](https://github.com/Deocy/the-study-of-spillover-effect-with-DCC-GARCH-model-in-R-programming/blob/master/spillover%20overview.png)

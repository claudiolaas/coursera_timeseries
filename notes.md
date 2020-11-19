Week 1 
- time series = stochastic process
- inferences = confidence intervals, hypothesis tests
- assumptions for linear regression: 
    - errors are normally distributed
    - have the same variance(homoscedastic)
    - are unrelated to eachother
- Asses Residuals: 
    - "histogram of residuals" only valid if you have lots of data points
    - QQ-Plot --> look for **systematic** deviations from the straight line
    - plot residuals over time --> inspect for patterns
- Framework for Hypothesis Test:
    - state variables
    - state null and alternative hypothesis
    - decide on a level of significance a (P(type I error))
    - compute a statistic (z,t,X^2)
    - find the p-value (probability to finding values this extreme without rejecting the null hypothesis)
    - form a conclusion --> p<a --> reject H0
- standard errro = standard deviation of a sample
- Covariance is unit dependent, Correlation is not
- (DataPoint-Mean)/std --> standard units

WEEK 2
- Stationarity (property of a stochastic process): 
    - no systematic change in mean --> no trend
    - no systematic change in variation
    - the properties of the TS of one section are the same of another section of the TS
    
- Random Variable = "machine" that produces numbers with a distribution, descrete or continuous
- Covariance = linear dependence between two random variables
- Stochastic Process = collection of Random Variables
- Time Series = realization of a stochastic process.
- Differencing to make a TS stationary: Xt - Xt-1 = purely random TS

WEEK 3
- An  individual  trajectory  of a TS corresponds  to  a realization of  a stochastic  process. The  set  of  all  possible trajectories is called the ensemble
- Stochastic Process: Family
𝑀𝑒𝑎𝑛𝐹𝑢𝑛𝑐𝑡𝑖𝑜𝑛:𝜇(𝑡)≡𝜇𝑡≡𝐸[𝑋(𝑡)] also written 𝐸[𝑋𝑡]
𝑉𝑎𝑟𝑖𝑎𝑛𝑐𝑒𝐹𝑢𝑛𝑐𝑡𝑖𝑜𝑛:𝜎2(𝑡)≡𝜎𝑡2≡𝑉[𝑋(𝑡)] also written 𝑉[𝑋𝑡]
𝐴𝑢𝑡𝑜𝑐𝑜𝑣𝑎𝑟𝑖𝑎𝑛𝑐𝑒𝐹𝑢𝑛𝑐𝑡𝑖𝑜𝑛:𝛾(𝑡1,𝑡2)≡𝐸[(𝑋(𝑡1)−𝜇(𝑡1))(𝑋(𝑡2)−𝜇(𝑡2))]
- to know the whole Stochastic process you have to know the whole joint distribution of all random Variables, not just one realization of the stochastic process
- assuming stationarity allows to "pool" results along a realization of a stochastic process
- scaling covariance to get autocorelation function p(t) = y(t)/y(0) (for stationary TS)
- Covariance only tells us if the slope is positive or negativ but not how steep it is
- Covariance is sensitive to scale (and thus hard to interpret)
- Covariance with itself is the same as the Variance
- Correlation = 1 means a straigt line goes through all data points
- Correlation does not tell us about the steepness of the slope
- Correlation = Covariance(X,Y) / (sqrt(var(X)) * sqrt(var(Y)))
- R-squared --> how much of the variance in the data is explained by the model
- Weak stationarity: constant mean  and Autocovariance Function only depends on lag spacing

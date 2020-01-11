# Climate-Project-Repo

CORE NULL HYPOTHESIS:  
- There is no relationship between sea level height and carbon dioxide.

CORE ALTERNATE HYPOTHESIS: 
- If there is an increase in carbon dioxide, then there is an increase in sea level height. 

METHODS: 

We obtained data for the following: water temperature, sea level height, atmospheric carbon dioxide, and tropospheric temperature for Scripps Pier in La Jolla.

- Performed t-tests on 4 sets of independent samples
- Ran linear regression for each set of samples
- Obtained Pearson correlation coefficient to show strength of linear relationship.

DISCUSSION:

1.From 1849 to 2013, the slope of the San Diego and global temperature trend is 0.0048 and 0.0068 degrees (C) per year, respectively.  Both trends are positive, albeit different. From 1969 to 2019, the slope of the San Diego temperature trend is 0.0276 degrees (C) per year. 
										(0.0276 ÷ 0.0048 = 5.75)
The global temperature is the average of the temperatures reported by 10 countries, which are located in the four world quadrants. 
 

2. Water Surface Temperature and Sea Levels. Our findings show that there is an upward linear trend in water surface temperatures as we progress through time. We performed a T-test for 2 independent samples 
								stats.ttest_ind(surface_y, sealevel_y, equal_var=False), 
in which the test statistic was found to be 148.93. The above function also provided us with our P-value, which was found to be much less than 0.05. The P-value is equal to 3.325e-68, which is statistically significant. We then ran the Pearson method for finding the correlation coefficient between the two series,
							values[['Surface Temperature', 'Height(m)']].corr(method="pearson").
The Pearson correlation coefficient r for sea level height and water surface temperature is 0.834, which is indicative of a strong linear relationship. Additionally, due to how extremely small the p-value is, we were able to reject the null hypothesis. Our findings show that as sea level height increases, there is an increase in water surface temperature.

3. CO2 levels and Water Temperatures. Average CO2 levels and water temperatures have both risen over the years by a significant amount. Since 2010, the growth rate appears to have accelerated in water temperatures rising. 

4. Sea Levels and Tropospheric Temperature. The individual t-test performed resulted in p-values close to zero, so the tests are statistically significant. 

5. Tropospheric Temperature and CO2. The pearson correlation coefficient between CO2  concentration and San Diego troposphere temperature (as displayed above) is 0.59, which indicates a positive linear relationship. 

6. The pearson correlation coefficient between mean sea level and CO2 levels is 0.43, which indicates a linear relationship.  

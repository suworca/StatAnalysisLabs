## Data
Source: sklearn.datasets.fetch_california_housing

# Task 
## Part 1:
Select the most significant factors and build the best model where the effective feature is MedHouseVal.

After that, build a similar model with purified emission data using the Tukey method (according to the selected factor characteristics).
## Part 2
Build 4 models based on the training sample:

1. The best (previously built), without the Population attribute; 
2. The best (previously built), with the logarithmized attribute Population; 
3. The model with pre-cleaned outliers without Population attribute; 
4. The model with pre-cleaned outliers with logarithmized Population attribute

Evaluate the results obtained from the test sample. Visualize the results.
# Results
According to the results of laboratory work No. 4, 4 models were obtained:

* Model with outliers and without Population factor,
* A model with outliers and with the inclusion of a logarithmized Population factor,
* A model purified from outliers by the D. Tukey method, and without the Population factor,
* A model purified from outliers by the D. Tukey method, and with the inclusion of a logarithmized Population factor.
All models were built based on training samples, and their characteristics were evaluated using raw test samples.

According to the R2 indicator, model No. 4 is the best. Almost the same result is observed in model No. 3. Therefore, according to the r^2 parameter, the best models are those cleared of emissions by the D. Tukey method.

According to the mean squared error indicator, the best models are models No. 1 and No. 2, they produce fewer gross errors. However, their r^2 is relatively low, so in the end we prefer model No. 4, since its mean squared error is less than the similar indicator of model No. 3.

In this case, other characteristics of the models should be considered to determine the best model. So, according to the indicators of the adjusted coefficient of determination, AIC, BIC, Log-Likelihood, model No. 4 is the best. This does not contradict the conclusion made above in terms of r^2 and mean squared error, so we choose it (an outlier-free model with a logarithmized Population parameter).
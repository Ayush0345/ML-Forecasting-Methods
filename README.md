# ML-Forecasting-Methods-for-House-Prices

I use XGBoost to forecast out-of-sample house prices in MSA counties (delineated via FIPS codes) in the United States. I used the dataset from **Lutz, Chandler and Sand, Ben, Highly Disaggregated Land Unavailability (February 10, 2023). Available at SSRN: https://ssrn.com/abstract=3478900 or http://dx.doi.org/10.2139/ssrn.3478900.**

The dataset contains points about FIPS codes, differenced and logged house prices in MSA counties, and a Land Unavailability Machine Learning Instrumental Variable (LU-ML IV). 

Performing XGBoost yields a difference of about **0.06%** in actual and predicted house prices with the actual prices being on the right tail of the distribution. The forecaster minimizes the mean squared error (0.000044) on the first stage regression of PanelOLS. _(I cannot reveal the details of the PanelOLS regression and the 3SLS results due to the ongoing nature of the project.)_

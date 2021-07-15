# Life-Expectancy(DATA ANALYSIS)
Can we correctly predict life expectancy? And, if so, which features are most relevant for prediction?

With 1,345 indicators across 20 categories for 60 years, the World Bank Data Bank is an invaluable resource to help us explore insigns about the life expectancy.
[worldbank-world-development-indicators](https://datacatalog.worldbank.org/dataset/world-development-indicators).


Using our updated dataset, we created a machine learning model in an attempt to forecast a more accurate prediction of life expectancy based on these indicators. As the data consisted of over a thousand indicators, we used Linear Regression as an exploratory starting point to analyse the original data (1960-2019). The idea was to infer causal relationships between the independent variable of ‘life expectancy’ and 21 mostly economic dependable variables.

We then filtered it further by identifying 19 more rounded (Social, Economic, Mortality and Health-Related) indicators which we felt were most correlated with life expectancy.  Moreover, for the purpose of our analysis, we narrowed our data for the time period of 1999 - 2019. 

For this dataset we applied the Gradient Boosting Regressor (GBR).  The GBR starts by fitting a decision tree model to the data.						
Finally, we built and deployed an interactive GBR machine learning model to predict life expectancy based on our 19 key indicators, during the period of 1999-2019.



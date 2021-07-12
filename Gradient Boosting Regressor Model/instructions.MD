# CSV Files

The original dataset was very tall, with one single row per country-year-indicator combination. For machine learning, the dataframe needs to be reshaped to have features (development indicators) as column headers and the countries as the rows. As a result, the main data wrangling steps were unstacking the data to structure it in a workable state.

While the datasets are fairly clean, there are missing data - for several years for some metrics, and large gaps for specific counties.

In this case we have sought to collate a more rounded dataset(from 1999-2019) which considers 19 social, economic, mortality and health-related indicators in which we considered to be essential for the calculation of life expectancy.
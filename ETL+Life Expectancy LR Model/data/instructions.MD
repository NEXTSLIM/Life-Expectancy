# CSV Files

The `CSV' files have not been included due to its size. In order to run the code you need to follow the instructions detailed below.

## Instructions

1. Go to the [worldbank-world-development-indicators](https://datacatalog.worldbank.org/dataset/world-development-indicators).

2. Download the Bulk Downloads `CSV`files if you want to perform the analysis. 
For this project this is the list of files:

- WDICountry.csv
- WDISeries.csv
- WDIData.csv

### DETAILS: 

Download WDI_csv.zip from https://data.worldbank.org/data-catalog/world-development-indicators
Unzipped the files

Performed the below in operations in Python 
<br>
import pandas as pd
<br>
import numpy as np
<br>
import matplotlib.pyplot as plt
<br>
import random
<br>
%matplotlib inline

wdi = pd.read_csv("WDIData.csv")
print(wdi.shape)
print(type(wdi))
names = wdi.columns.values
print(names)

#Transpose the year and thier values
<br>
wdi_new = pd.melt(wdi, id_vars=['Country Name', 'Country Code', 'Indicator Name', 'Indicator Code'], var_name="Year", value_name="Value") 
wdi_new.shape
<br>
new dataframe created
wdi_new.head() 

I could see that the columns for each year are transposed to rows.


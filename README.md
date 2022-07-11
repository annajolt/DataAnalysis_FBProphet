# Forecasting Net Profits
---
## *Necessary Library Installs*

- import pandas as pd
- import holoviews as hv
- from fbprophet import Prophet
- import hvplot.pandas
- import datetime as dt
- import numpy as np
- from pathlib import Path
- %matplotlib inline

***Please Note that this notebook and analysis was done through a Google Colab Notebook.***

## *Analysis*

Because the analysis will be conducted in a Google Colab Notebook, you will need to cofigure the worskspace and connect your data to your Drive. This is done by mounting the Drive into the Notebook:


```
# Upload the "google_hourly_search_trends.csv" file into Colab, 
# then store in a Pandas DataFrame
# Set the "Date" column as the Datetime Index.
from google.colab import drive
drive.mount('/content/drive')
```
Once this is done, you create a ```file_path``` to your file  and read the csv into a Pandas DataFrame.

There are mutliple steps to be done for the analysis of Mercado Libre, and the first one was for locating possible patterns of Google Search trends. 

It was evident that searches of Mercado increased during specific days in a week and even hours. The below graph shows the weekly search trends of Mercado as well as the heatmap to show 

![Mercado_Weekly_Search Trends]("../Resources/Mercado_search_trends_weekly.png")


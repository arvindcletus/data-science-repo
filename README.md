# An Analysis of Airbnb Data from London

## Focus of the Analysis

In this analysis, three questions were posed:

1. Which neighbourhoods have the most expensive listings in London?
2. What features influence the price of an Airbnb listing?
3. What is the percentage of positive reviews for the top 20 most reviewed listings in London?

## Files in this Repository

### Data Files
Two data files used in this analysis:
- listings.csv
- reviews.csv

### Files for Plotting a Choropleth Map
The folder named gis-files contains files for plotting a choropleth map of London.

## Libraries Used

```
import numpy as np
import pandas as pd
import re
import matplotlib.pyplot as plt
import geopandas as gpd
from shapely.geometry import Point, Polygon
import folium
import seaborn as sns
from lightgbm import LGBMRegressor
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split, KFold, cross_val_score
from sklearn.metrics import accuracy_score, mean_squared_error, r2_score
from xgboost import XGBClassifier
from sklearn.ensemble import RandomForestRegressor
from nltk.sentiment.vader import SentimentIntensityAnalyzer
```

## Summary of the Results

1. An analysis of the dataset reveals that the median rental prices of certain neighbourhoods or boroughs are higher than others. 
2. The features that have the highest impact on the price of an Airbnb listing are the number of bedrooms, the room type (private rooms fetch a higher price), the location and the number of guests the property can accommodate.
3. A sentiment analysis of the reviews finds that most reviews tend to be positive. 


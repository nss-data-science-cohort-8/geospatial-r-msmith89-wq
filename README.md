# Analyzing Aggravated Burglaries in Davidson County

### Part 1 - Burglaries

You've been provided three datasets for this project:
* burglaries_2023.csv: Contains data on the aggravated burglary incidents in Davidson County. This was obtained from https://experience.arcgis.com/experience/060537e33bff45d996ca09f84a4eb0a6/.
* census.csv: Census tract level data on population and median income. This was obtained from the US Census American Community Survey.
* DC: A shapefile containing Davidson County census tracts

Perform a spatial join to determine the census tract in which each burglary occurred.

### Part 2 - Exploratory Analysis

Now, merge in the census data. **Note:** Make sure that the final dataset contains all census tracts (there are some census tracts that had no burglaries).

Perform some exploraty analysis on your prepared dataset.

Aggregate the data by census tract. **Warning:** each incident can appear multiple times if there are multiple victims, so be sure that you aren't double-counting any incidents. 

Which census tract had the highest number of burglaries? Which census tract had the highest number of burglaries per 1000 residents? 

Finally, look at the relationship between median income and number of aggravated burglaries per tract. How would you describe this relationship?

### Bonus: Statistical Modeling

Fit a Poisson regression model with target variable the rate of burglaries per census tract and with predictor the median income. Offset using the log of the population so that we are looking at the rate of burglaries per population instead of the number of burglaries. How can you interpret the meaning of the output? How do the estimates from the model compare to the observed data?

Additional Resources for Generalized Linear Models:
* [Generalized Linear Models in R](https://app.datacamp.com/learn/courses/generalized-linear-models-in-r), a DataCamp course
* [Beyond Multiple Linear Regression, Chapter 4](https://bookdown.org/roback/bookdown-BeyondMLR/ch-poissonreg.html)

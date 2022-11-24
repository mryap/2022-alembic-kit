---
layout: post
title: "Handling Missing Data with Code"
date: 2018-09-16
categories:
- Data Science
---

A missing data solution has two goals:

- minimal loss of statistical power
- unbiased estimates and standard errors.

Which missing data solution you take depends in part on the distribution of missing data and the analyses you'll be doing.

The default “solution” is listwise deletion, which means you drop any case with a missing value. Listwise deletion and complete case analysis are two names for the same concept. For listwise deletion to not cause bias, all missing data must be missing completely at random.

2 Recommended Solutions for Missing Data: Multiple Imputation and Maximum Likelihood

Maximum likelihood works very well for missing data and requires no extra work, but can only be used in certain models. If you’re running a linear or log-linear model, (like a regression or linear mixed model), maximum likelihood techniques give the same great, unbiased, uninflated, full power results that multiple imputation does.

Mean substitution is about the worst thing you can do for missing data.

A data analyst worth his or her salt will report which missing data technique used and why.

## Handle missing data with SQL, R and Python

You can leave the data as is and go for a model which can handle missing data (such as XGBoost, Random Forest).  For some machine learning algorithms such as Linear Discriminant Analysis (**LDA**), having missing values in a dataset can cause errors.

### SQL

In SQL, NULL represents a missing or unknown value. You can check for NULL values using the expression IS NULL. For example, to count the number of missing birth dates in the people table:
```sql
SELECT COUNT(*) FROM people WHERE birthdate IS NULL;
```


### R
There is a R package dealing with missing data named Amelia (yes after the famous missing Aviator)
```python
install.packages("Amelia", repos="http://r.iq.harvard.edu", type = "source")

```


### Python

```python
from pandas import read_csv
import numpy
dataset = read_csv('pima-indians-diabetes.csv', header=None)
# mark zero values as missing or NaN
dataset[[1,2,3,4,5]] = dataset[[1,2,3,4,5]].replace(0, numpy.NaN)
# print the first 20 rows of data
print(dataset.head(20))
```

![](https://i.etsystatic.com/5516807/r/il/007a20/229305972/il_570xN.229305972.jpg)
*Source: [Etsy Listing](https://www.etsy.com/listing/70557200/statistics-propaganda-poster-missing)*
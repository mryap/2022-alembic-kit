---
title: Sessions Quality in Google Analytics
date: '2018-09-30 11:38:00'
excerpt: >-
  SQ metrics bring Google’s machine learning capabilities to predict the
  likelihood of a user making a transaction on a website. 
template: post
---
Sessions Quality  is an estimate of how close a particular session was to transacting, ranging from 1 to 100, calculated for each session. A value closer to 1 indicates a low session quality, or far from transacting, while a value closer to 100 indicates a high session quality, or very close to transacting. A value of 0 indicates that Session Quality is not calculated for the selected time range. 

Under Bigquery, the field is `totals.sessionQualityDim`

### What you can do with Sessions Quality?

Sessions quality show signs of high consideration or purchase intent.  It allows you to build New Remarketing Segments. By creating segments with high Session Quality in Google Analytics, you are then able to push these out to AdWords and target them within re-marketing campaigns.

Finding Bot Traffics - Session quality reports make it easier to remove bots from reports: simply create a segment where quality equals 1. 

### What else is there that I should know?

The SQ metrics bring Google’s machine learning capabilities to predict the likelihood of a user making a transaction on a website.  The Google algorithm, based on the selected data sample, learns the process that leads to the declared goal - in this case, e-commerce transactions. Thanks to this, it is able to evaluate a fresh sample of data and assess their potential. Therefore, it is important that the sample is representative. This results in certain minimum requirements, the threshold determined in the case of **Session Quality** is:

* 1000 e-commerce transactions a month
* Maintain this level for the next 30 days

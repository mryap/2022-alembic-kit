---
title: Ireland Milk Trade in 2015
date: 2017-11-22 12:22:15 +00:00
author: mryap
categories:
- Open Data
---

The United Nations Comtrade database used to analyse Ireland's imports and exports of milk and cream in 2015:




  * How much does Ireland export and import and is the balance positive (more exports than imports)?


  * Which are the main trading partners, i.e. from/to which countries does Ireland import/export the most?


  * Which are the regular customers, i.e. which countries buy milk from Ireland every month?


  * Which countries does Ireland both import from and export to?




## Getting and preparing the data


The data is obtained from the [United Nations Comtrade](http://comtrade.un.org/data/) website, by selecting the following :




  * Type of Product: goods


  * Frequency: monthly


  * Periods: January to May of 2015


  * Reporter: Ireland


  * Partners: all


  * Flows: imports and exports


  * HS (as reported) commodity codes: 0401 (Milk and cream, neither concentrated nor sweetened) and 0402 (Milk and cream, concentrated or sweetened)













## Accessing data through APIs
























The data can also be downloaded directly from Comtrade using the "View API Call" URL, modified in the following ways:




  * `max=500` is increased to `max=5000` to make sure all data is loaded,


  * `&fmt=csv` is added at the end to obtain the data in CSV format.


  * `&r=372` is the ID code for Ireland [https://comtrade.un.org/data/cache/reporterAreas.json ](https://comtrade.un.org/data/cache/reporterAreas.json)




## Conclusions


The milk and cream trade of Ireland from January to May 2015 was analysed in terms of which countries Ireland mostly depends on for income (exports) and goods (imports).

Over the period, Ireland had a trade deficit of over 15 million US dollars.

UK is the main partner, but it imported from the UK almost the triple in value than it exported to the UK.

Ireland exported to over 58 countries during the period, but only imported from 5 countries, the main ones (top 5 by trade value) are China, UK, Netherland, Nigeria, Algeria. UK and Netherland being geographically close.

Ireland has bi-directional trade (i.e. both exports and imports) with 15 countries. Singapore is the only country that geographically furthest away.

[Data Analysis Code on GitHub ](https://github.com/mryap/src/blob/master/un-comtrade/Ireland-2015-5Month-Milk.ipynb)











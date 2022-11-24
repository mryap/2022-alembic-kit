---
title: Ingesting New Datasets into BigQuery
date: 2019-04-20 
description: What I learn from created a new dataset and ingested new external data sources into BigQuery from CSV, Google Cloud Storage, and Google Drive.
#image: "/img/measurement-in-mutli-screen-world5.jpg"
categories:
-  BigQuery
---

What I learn from ingesting new external data sources into BigQuery from CSV, Google Cloud Storage, and Google Drive.

Linking external tables to BigQuery (e.g. Google Spreadsheets or directly from Google Cloud Storage) has several limitations. Two of the most significant are:

- Data consistency is not guaranteed if the data values in the source are changed while querying.
- Data sources stored outside of BigQuery lose the performance benefits of having BigQuery manage your data storage (including but not limited to auto-optimization of your query execution path, certain wildcard functions are disabled, etc.).

Data from external tables do not get the advantage of metadata stored and cached in BigQuery.  BigQuery needs to query the external source each time you need to read data even if you are running the exact same query -- since caching is not used for external sources.
[link](https://cloud.google.com/bigquery/external-data-sources#external_data_source_limitations)


You will need to extract the spreadsheet ID from the document link before BigQuery will accept it. 

If the Sharable Link is 
`https://docs.google.com/spreadsheets/d/1TPSjzfPrs9vsc4Im2JWnhE3GJ9NVHwhJWRMpUkQDSyw/edit?usp=sharing`,
The Spreadsheet ID is `1TPSjzfPrs9vsc4Im2JWnhE3GJ9NVHwhJWRMpUkQDSyw`

https://drive.google.com/open?id=1TPSjzfPrs9vsc4Im2JWnhE3GJ9NVHwhJWRMpUkQDSyw
---
title: Google Analytics App+Web - The new Google Analytics
subtitle: Updated on 15th Oct 2020 as Google Analytics App+Web are out of beta
date: 2020-10-13T22:10:23.496Z
thumb_img_path: /images/screenshot_2020-10-21-analytics-1-.png
template: post
---
As on 14th Oct 2020, Google Analytics App + Web are out of beta. It known as Google Analytics 4.

Why 4? I think if you exclude Urchin, which was acquired by Google in April 2005, this is the 4th major iterations. 

![](/images/april-2005.png)

GA4 is combination of (App + Web and Google Analytics for Firebase)

Introduce in July 2019, Google Analytics App+Web  data collection and analysis is based on the Event-Driven Data Model.  This model allows you to track *everything* as events, regardless of the platform - whether App or Web. Event-Driven Data Model itself is not new. Heap Analytics and Facebook Analytics are already in this Event-Driven Data Model of data collection. 

![A screenshots of the new Google Analytics dashboard ](/images/screenshot_2020-10-15-analytics-home.png "No more page view metrics. ")

## What Others Said

<!--StartFragment-->

I read all the blog post out there on Google Analytics 4 (GA4). Here my summary

* GA4 lets marketers understand what happens on their digital properties while respecting GDPR, ITP & user awareness about tracking and privacy
* The previous Acquisition Report in Google Analytics will split between User Acquisition (First Touch) and Traffic Acquisition. (the old Default Channel Grouping report). This the move from Channel focused ‘Last Touch Attribution’. 
* GA 4 do away the page view/screen view concept with a flexible system of events and parameters (aka event-driven data model). The event-driven data model works for websites and mobile apps
* 3 new metrics are introduced: Engaged Sessions” (in “Behavior” report), which removes bounces, “Engaged Sessions per User” and “Engagement Time”
* GA 4 comes with automatic event tagging for user scroll tracking, youtube video interactions, clicks to exit the site. (I used to provide value-add srrvices to code for event tagging)
* You can now use GA4 data with BigQuery without the USD 150,000 GA360. BigQuery, a Google Marketing Data warehouse opens up the availability to export raw, unsampled Google Analytics data. This allows business with advanced web analytics needs to integrating with CRM
* Google Data Studio has a direct connector into your GA4 property. No need to go through [BigQuery ](https://www.testandoptimize.com/posts/2019-03-18-things-to-know-about-bigquery/)to get your unsampled data into your data visualization tool
* With Google Analytics 4, the old tracking code (analytics.js) is no longer supported, only GA4 and gtag.js are supported going forward.

## What about Google Analytics?

Google official line is

> We recommend continuing to use your existing Analytics properties alongside an App + Web property.

When I was hired for web analytics project, I always set up Google Analytics App+Web together with Google Analytics.

## Force multiplication

A feature of GA4 I am excited about is BigQuery Export.  BigQuery export opens up the availability to export all the raw, un-sampled Google Analytics data. This allows business with advanced analytics requirements like integrating with other datasets such as CRM, external third-party data access to a datawarehouse without dedicated IT department. 

With data stored in the cloud, you can access and manipulate data in Google BigQuery with Python and R. These 2 languages make it easier to build a statistical model which can be used for various purposes – understanding customers’ in-app behavior, predicting the churn rate, etc. 

I being up to speed with Google BigQuery since 2019. Hire me with confidence. 

https://www.qwiklabs.com/public_profiles/fdf93c0d-bc8b-4952-b7fe-1dade1d6e917

https://www.coursera.org/account/accomplishments/specialization/PKU7C2X2QRG8
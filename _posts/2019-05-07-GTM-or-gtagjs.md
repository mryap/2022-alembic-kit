---
title: Google Tag Manager (GTM) or Global Site Tag (gtag.js)?
date: 2019-05-07 
description: Google Tag Manager (GTM) or Global Site Tag (gtag.js)? 
#image: "/img/measurement-in-mutli-screen-world5.jpg"
categories:
-  GTM
---

Google Tag Manager is a robust and full-featured tag management system, which supports Google and 3rd party tags(Facebook conversion pixels or heatmapping tool tags). 

In 2018, Google updated their tracking code from `analytics.js` to gtag.js (known as the Global Site Tag)

Difference between Universal Analytics (Analytics.js) And Global Site Tag (gtag.js)

- Universal Analytics tracking (analytics.js) only supports Google Analytics but Global Site tag (gtag.js) can support as many Google platforms as you require, e.g. Google Analytics, Google Ads or Firebase tracking.
- Analytics.js uses trackers to send data to Google Analytics and (2) hit types to specify the types of the data. Gtag.js doesn’t use trackers to send data to Google Analytics- it sends data to Google platforms, identified by their tracking IDs set by the config command. The event names supplied to gtag.js specify the types of data being sent to Google Analytics.
- Analytics.js and Gtag.js both use a different type of tracking parameters.
- Unlike universal analytics tracking, Global site tag can be used for conversion tracking.
- Global site tag can be used for remarketing as well but Universal Analytics can’t.

`gtag.js` is a script that allows you to send data to only Google Marketing Platform (Google Ads, Campaign Manager, Display & Video 360, Search Ads 360, and Google Analytics) It will not work with non-google products like Facebook conversion pixels or heatmapping tool tags(the so-called "3rd party tags")

![](https://res.cloudinary.com/mryap/image/upload/v1557327756/global-site-tag.jpg)

Your gtag.js snippet would look like this if you’re using Google Analytics and Google AdWords together

 ~~~
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-1234567-8');
  gtag('config', 'AW-1234567-8');
</script>
 ~~~

For product-specific documentation related to gtag.js, refer to the following:

- [Google Analytics](https://developers.google.com/analytics/devguides/collection/gtagjs/)
- [Remarketing](https://support.google.com/google-ads/answer/2454000)
- [Google Ads conversions](https://support.google.com/google-ads/answer/1722022)
- [Campaign Manager and Display & Video 360 know also as DCM](https://support.google.com/dcm/partner/answer/7568534)
- [Search Ads 360](https://support.google.com/searchads/answer/7550511)

### What does this means?

If you are a website owner that do not deal with code, you do not need to worry about. Hire me, a marketing analytics developer to deal with this. 

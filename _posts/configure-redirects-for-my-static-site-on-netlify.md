---
title: Configure Redirects for my static site on Netlify
date: 2020-03-09T09:19:48.817Z
template: post
---
Redirect is the web’s version of a post office staff who has to collect mail from one address and deliver it to another. 

There are times when further steps are required for successful mail delivery. For instance, if a person moves, the post office staff must be notified of this change so the mail can be successfully “redirected” via a change of address.

I being publishing on hireyap.netlify.com for 17 months. By default, any site on Netlify is accessible via its Netlify subdomain, which has the form `[name-of-your-site].netlify.com`. 

Netlify is a service for quickly rolling out static websites. The use of GitHub has becomes the way of operating.  

I decide to use my personal domain for the Netlify site. Known as Custom domains, it allow others to make your sites accessible at your own, choosen non-Netlify domain names (in my case it www.testandoptimize.com)

The way it works involve the process of editing the Redirect rules on Netlify configuration file - netlify.toml file , push (upload) to Github and revisit the site the next day. 

The code are here

```
[[redirects]]
  from = "/"
  to = "https://www.testandoptimize.com/"
  status = 301
  force = true
  headers = {X-From = "Netlify"}
```

The redirect from subdomain on netlify (hireyap.netlify.com) to my own Custom Domains. (www.testandoptimize.com) took about 16 hours. 

I doing this as people typing https://www.testandoptimize.com/ in search engine might click on the first result which I do not want visitors to go to. 

![](/images/screenshot_2020-03-09-testandoptimize-com-google-search.png)
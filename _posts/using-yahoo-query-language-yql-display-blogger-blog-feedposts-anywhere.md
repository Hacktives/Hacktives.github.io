---
title: 'Using Yahoo Query Language YQL Display Blogger Blog Feed/Posts Anywhere'
date: 2017-02-27T08:00:00.000-08:00
draft: false
url: /2017/02/using-yahoo-query-language-yql-display.html
tags: 
- Resources
- Learn
---

Ever since Google shut down their free feed API service late December 2016, Blogger users have contacted us in finding out on any alternatives which is more stable, reliable & most important clean API's to retrieve blog feed data publicly - most important FREE!  
  

[![Display Blogger feed use Yahoo!QL with AMP iframe for Blogspot Template](https://2.bp.blogspot.com/-DYnp7uXb1V0/WKP2_hqw5gI/AAAAAAAAhCs/nEVRDd26bycVgTuOc0idrBe-fYRskTKLQCLcB/s640/Yahoo%2521%2BQuery%2BLanguage%2BYQL%2Bdisplay%2BBlogger%2BPosts%2BAnywhere%2Bwith%2BAMP%2BHTML.png)](https://2.bp.blogspot.com/-DYnp7uXb1V0/WKP2_hqw5gI/AAAAAAAAhCs/nEVRDd26bycVgTuOc0idrBe-fYRskTKLQCLcB/s1600/Yahoo%2521%2BQuery%2BLanguage%2BYQL%2Bdisplay%2BBlogger%2BPosts%2BAnywhere%2Bwith%2BAMP%2BHTML.png)

  
Reasons were:  
  

1.  Many of their Blogger plugins was hosted on domain outside of their blog which when using javascript (to send/retrieve data cross domain) as-is would not be possible.
2.  Issues with Blogger blogs with HTTP & HTTPS protocols due to browser security & restrictions.
3.  Returns/receive datas which can be easily manipulated/process.
4.  Developing an AMP iframe to deploy/display blog feed which requires HTTPS connection & compatible with HTTP protocol.

  
Here's [Yahoo! Query Language](https://developer.yahoo.com/yql/) (YQL), from Yahoo! developer website...  
  

> The YQL (Yahoo! Query Language) platform enables you to query, filter, and combine data across the web through a single interface. It exposes a SQL-like syntax that is both familiar to developers and expressive enough for getting the right data.

  
Since that YQL provides JSON data format as data output, makes it easier for Blogger template developers/designers to retrieve datas - just like how they normally would retrieving JSONp datas using Blogger's blog internal data feed API.  
  
Below is an example how to use YQL using **plain/pure javascript**, process data & output Blogger feed data to HTML. This script can be hosted on a different domain with HTTP or HTTPS  (works best for compatibility) protocols for any Blogger blogs (with or without HTTPS enabled).  
  
[Continue](https://blogr-amp.blogspot.com/2017/02/using-yahoo-query-language-yql-display.html#more)
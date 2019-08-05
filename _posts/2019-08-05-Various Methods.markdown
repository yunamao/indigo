---
title: "Various methods"
layout: post
date: 2019-08-05 18:28
image: /assets/images/markdown.jpg
headerImage: false
category: blog
author: yunamao
description: 操作流程
---

### 1. <strong> statistical method </strong><br>
  (1) Detrend：

Detrending is removing a trend from a time series; a trend usually refers to a change in the mean over time. When you detrend data, you remove an aspect from the data that you think is causing some kind of distortion. For example, you might detrend data that shows an overall increase, in order to see subtrends. Usually, these subtrends are seen as fluctuations on a time series graph.<br>

Removing a trend from the data enables you to focus your analysis on the fluctuations in the data about the trend. A linear trend typically indicates a systematic increase or decrease in the data. A systematic shift can result from sensor drift, for example. While trends can be meaningful, some types of analyses yield better insight once you remove trends.<br>

Whether it makes sense to remove trend effects in the data often depends on the objectives of your analysis.

matlab:<br>
y = detrend(x) to remove the best straight-line fit from vector x.<br>
y = detrend(x,’constant’) to remove the mean value from vector x.<br>
y = detrend(x,’linear’,bp) to remove a continuous, piecewise linear trend from vector x.)<br>
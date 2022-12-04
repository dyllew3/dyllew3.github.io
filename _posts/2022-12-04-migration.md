---
layout: post
title: Migration for data collection on dublin airport security times
date: 04/12/2022
---

So I had been using the free heroku instance that I had access to to run the data collection.
However recently that service was has been shut down https://blog.heroku.com/next-chapter and I have had to move to AWS lambda,
making use of their free tier along with the fact I have 25 dollars worth of credits.
So I should be able to keep the data collection running for the foreseeable future.
Another modfication to the code I had to make was instead of it being a service that runs constantly
but only performs data colleciton every 10 minutes now it will run on lambda once but that lambda function
is triggered every 10 minutes.


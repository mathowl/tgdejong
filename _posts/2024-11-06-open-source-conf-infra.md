---
layout: post
title: Open source digital infrastructure for conference
date: 2024-11-06 08:51:00-0400
description: building open source web-services for conferences
tags: java opensource
categories: code
related_posts: false
---

For mid-size conferences (O(100)) it can be troublesome to build the digital infrastructure. I suspect that a lot of institutes will unnecessarily resort to paid-subscription services. I think the money could be put towards better use. So I am building some generic opensource code that future organizers can easily use.

I am trial running it for [this conference](https://sites.google.com/view/deds2025/home). As small things get continuously added I will release it after the conference. 

The overall framework is to have participants complete registration through a google form which collects the data in a google sheet on which an app-script (=serverside java) sits. The app-script performs operations based on triggers that are activated in the google sheet via checkboxes by organizers. Here the automization includes generic personalized emails and personalized invitation letters. 

The convenient thing is that all of this can be run through ordinary free-to-use google services. So essentially you can clone the files to your google-drive and you are ready to go.
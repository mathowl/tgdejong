---
layout: post
title: Improving speed of LLG reservoir simulations  
date: 2023-10-25 09:56:00-0400
description: accepted at MLNCP (NeurIPS)
tags: reservoir, coding 
categories: paper
giscus_comments: false
related_posts: false
related_publications: de2023mlncp
---

**Title** Virtual reservoir acceleration for CPU and GPU: Case study for coupled spin-torque oscillator reservoir 

 **Abstract** We provide high-speed implementations for simulating reservoirs described by $N$-coupled spin-torque oscillators. Here $N$ also corresponds to the number of reservoir nodes. We benchmark a variety of implementations based on CPU and GPU. Our new methods are at least 2.6 times quicker than the baseline for $$N$$ in range 1 to $$10^4$$. More specifically,  over all implementations the best factor is 78.9 for $$N=1$$ which  decreases to 2.6 for $$N=10^3$$ and finally increases to 23.8 for $N=10^4$.  GPU outperforms CPU significantly at $$N=2500$$. Our results show that GPU implementations should be tested for reservoir simulations. The implementations considered here can be used for any reservoir with evolution that can be approximated using an explicit method. 
---
layout: post
title: 1D intuitive asymptotic stabilty proof
date: 2023-12-29 08:51:00-0400
description: 
tags: ODE
categories: math
related_posts: false
---


So suppose we have an equation of the form 

$$
\dot y = f(y)
$$

with $$ y(t) \in \mathbb{R} $$, $$ f(0) = 0 $$ and $$ f \in C^1(\mathbb{R}) $$. Let's assume that $$ f $$ is of the form such the phase space is as in the figure below.

<div class="container">
        {% include figure.html path="assets/img/9.jpg" %}
</div>



These conditions on $$ f $$ allow us to show asymptotic stability of the equilibrium at 0. 



This set up will allow you to consider equations of the form 

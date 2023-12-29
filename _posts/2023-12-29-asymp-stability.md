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

with $$ y(t) \in \mathbb{R} $$, $$ f(0) = 0 $$ and $$ f \in C^1(\mathbb{R}) $$. Let's assume that $$ f $$ is of the form such that in some interval $$ (-a, a) $$ the phase space is as in the figure below.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/asymp.PNG" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    1D phase space
</div>


These conditions on $$ f $$ allow us to show asymptotic stability of the equilibrium at 0. 

$$

$$

**Stability.** Without loss of generality take $$ \varepsilon < a $$ and denote by $$ y(t; c ) $$  a solution which at t=0  is c .  If $$ |c| < \varepsilon $$ then $$ |y(t;c)| \leq |c|  < \varepsilon $$  for $$ t \geq 0 $$ because of the sign of $$ f $$ .

**Asymptotic.** Let's consider $$ 0 < c < \varepsilon < a $$ and again consider $$ y(t;c) $$ as previously defined. By the sign of $$ f $$ , $$ y(t;c) $$ is monotonously decreasing (with respect to $$ t $$). Therefore, $$ \lim_{t \rightarrow \infty } y(t;c) = b $$. If $$ b=0 $$ we are done so suppose $$ b > 0 $$. But then $$ f(b) <0 $$ so it hasn't converged which gives a contradiction. Hence, we obtain $$ b=0 $$. Same method works for $$ 0 > c > \varepsilon > -a $$ and for $$ c=0 $$ it is automatically satisfied. 

This set up will allow you to consider cases for which standard linearization techniques do not apply like $$ f(y) = -y^3 + y^4 g(y) $$ with $$ g \in C^1(\mathbb{R}) $$. Note that this approach only works in the 1D case. It is a nice exercise to check where it breaks down.   
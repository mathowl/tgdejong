---
layout: post
title: Neat 2D ODE transformations
date: 2023-12-09 20:51:00-0400
description: Generalizing neat examples
tags: math
categories: math
related_posts: false
---

I was teaching an ODE course last quarter and I came up with some fun exercises. I first asked the students to find the solutions for

$$
\begin{aligned}
\dot{x} &= 2xy \\
\dot{y} &= x^2+y^2
\end{aligned}  
$$

The trick here is consider new variables: $$ z_1 = x+y, z_2=x-y $$ The equations then become 

$$
\begin{aligned}
\dot{z}_1 &= z_1^2 \\
\dot{z}_2 &= -z_2^2
\end{aligned}  
$$

which are easy to solve. Then I gave the students this ODE

$$
\begin{aligned}
\dot{x} &= 2xy \\
\dot{y} &= x^2+4y^2
\end{aligned}  
$$

If you proceed as in te first problem you are going to have a hard time. A better way is to consider the new variable $$ z = y/x^2 $$ and we obtain that $$ \dot{z} =  1 $$ and then with some creative substituting you get there.

If we would consider a more general ODE

$$
\begin{aligned}
\dot{x} &=  \alpha xy \\
\dot{y} &= \beta x^2+ \gamma y^2
\end{aligned}  
$$

with $$ \alpha, \beta, \gamma $$ real parameters. Then it is easy to show that the first method works for  $$ \beta = \gamma $$ , $$ \alpha= -2 \beta $$. The second method works for $$ \gamma = 2 \alpha $$.

So far I haven't uncovered any other general case other then degenerate case obtained by setting a parameter to zero. I would love to know if this is part of some general theorem.

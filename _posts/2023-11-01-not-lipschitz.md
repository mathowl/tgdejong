---
layout: post
title: Not lipschitz but unique solutions 
date: 2023-11-01 11:12:00-0400
description: a neat example
tags: ODE
categories: math
related_posts: false
---

Just testing out MathJax 3 with a lovely example. Consider

$$
\frac{dy}{dt} = \sqrt{y}+1 \;\; y(0)=0 \;\; t \in [0,1] \;\; (y(t) \in \mathbb{R})
$$

We will show that solutions are unique eventhough it is not Lipschitz. There are multiple ways to solve this.  First of all we need to make sure that a solution exists. $$ \sqrt{y}+1 $$ is continuous in a neighbourhood of zero Hence, a solution exists. Let's write the differential equation in its integral form


$$
\begin{aligned}
\int^{y}_0 \frac{ds}{\sqrt{1+s}} &= \int^{t}_0 1 d\tau \\
\int^{y}_0 \frac{ds}{\sqrt{1+s}} &= t
\end{aligned}  
$$

For convenience let's define $$ G(z) = \int^{z}_0 \frac{ds}{\sqrt{1+s}} $$ ($$ G: \mathbb{R} \rightarrow \mathbb{R} $$). Observe that $$ G $$ is an increasing function. Therefore, for all $$ t $$ there exists at most one $$ z $$ such that $$ G(z) = t$$. 

Note that MathJax 3 is [a major re-write of MathJax](https://docs.mathjax.org/en/latest/upgrading/whats-new-3.0.html) that brought a significant improvement to the loading and rendering speed, which is now [on par with KaTeX](http://www.intmath.com/cg5/katex-mathjax-comparison.php).

---
# title for above
title: "Mltestscore 2017"
date: 2022-12-17T22:10:41+01:00
draft: false
rating: 5
identifyer:
  - doi: doi:10.1109/bigdata.2017.8258038
  - url: https://ieeexplore.ieee.org/abstract/document/8258038
# full title of resource
link_title: "The ML test score: A rubric for ML production readiness and technical debt reduction"
pubDate: "15 January 2018"
authors:
  - Eric Breck
  - Shanqing Cai
  - Eric Nielsen
  - Michael Salib
  - D. Sculley
difficulties:
  - advanced
linktypes:
    - paper
tags:
    - explainability
    - training pipelines
    - deployment pipelines
    - feature engineering pipelines
    - model serving
    - monitoring
    - automation
    - versioning
    - ml design
    - fundamentals
---

## The ML test score: A rubric for ML production readiness and technical debt reduction
Is a conference paper by 4 google authors and can be found at scihub or [IEEE](https://ieeexplore.ieee.org/abstract/document/8258038)

Abstract: 
> Creating reliable, production-level machine learning systems brings on a host of concerns not found in small toy examples or even large offline research experiments. Testing and monitoring are key considerations for ensuring the production-readiness of an ML system, and for reducing technical debt of ML systems. But it can be difficult to formulate specific tests, given that the actual prediction behavior of any given model is difficult to specify a priori. In this paper, we present 28 specific tests and monitoring needs, drawn from experience with a wide range of production ML systems to help quantify these issues and present an easy to follow road-map to improve production readiness and pay down ML technical debt.

![](/img/breck2017-tradit-vs-ml.png)

scope:
>  In this paper, we are largely concerned with supervised
ML systems that are trained continuously online and perform
rapid, low-latency inference on a server. 


Contains 
- 7 data tests
- 7 model tests
- 7 ml infrastructure tests
- 7 monitoring tests

Checking those items gives you a score of how mature your system is. 

## what do I think about it

Amazing overview of kinds of tests and control you can apply to systems.
Interesting things: they surveyed within Google, which has rigourous engineering standards, and even there "none of these tests was implemented by more than 80% of teams". 

I think this paper can inspire and improve your mlops game. 

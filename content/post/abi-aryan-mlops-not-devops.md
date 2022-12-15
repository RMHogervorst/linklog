---
# title for above
title: "Abi Aryan Mlops Not Devops"
date: 2022-12-04T11:31:57+01:00
draft: false
rating: 3
identifyer:
  - url: https://www.adventofdata.com/mlops-isnt-devops-for-ml/
# full title of resource
link_title: "MLOps isn’t DevOps for ML!"
pubDate: "1 December 2022"
authors:
  - Abi Aryan
difficulties:
  - intermediate
linktypes:
    - blogpost
tags:
  - mlops
  - devops
  - model versioning
  - training pipelines
  - deployment pipelines
  - monitoring
---

## MLOps isn’t DevOps for ML!
Is a blogpost and can be found here(https://www.adventofdata.com/mlops-isnt-devops-for-ml/)

> The big talent gap in the MLOps market can be easily and abundantly filled by DevOps practitioners in the conventional software world. After all, isn’t AI/ML just Software 2.0? 

> Machine learning models, as they are, require plenty of continuous human engineering at all stages from requirement engineering to data drafting to feature engineering to model deployment to observability and monitoring, given the data drift and unforeseen data samples that weren’t captured while training the model. This has created a massive debate in the machine learning community about how often we need to re-train our models in production as well as failsafe practices when something goes wrong. While clearly-defined immutable problems like detecting cats vs dogs can be far easily solved using neural networks however making even a preliminary medical diagnosis on patients in a single clinic requires humans in the loop.


> While most data science/machine learning practitioners tend to define MLOps as “the set of practices that aims to deploy and maintain machine learning models in production reliably and efficiently”. This consists of a continual loop of
- data collection and labeling
- experimentation to improve ML performance
- evaluation throughout a multi-staged deployment process
- monitoring of performance drops introduction

## what do I think about it
I actually never heard about software 2.0 "the code that doesn’t require explicit programming".
I think there are small, well-defined problems that can use of the shelf ML models that never have to be retrained. But for many problems a periodic retraining is necessary. 

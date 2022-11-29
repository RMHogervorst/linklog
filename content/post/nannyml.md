---
# title for above
title: "Nannyml"
date: 2022-11-28T11:08:24+01:00
draft: false
rating: 3
identifyer:
  - url: https://github.com/NannyML/nannyml
# full title of resource
link_title: Nanny ML
authors:
  - NannyML
difficulties:
  - advanced
linktypes:
    - website
tags:
  - model performance
  - concept drift
  - data drift
  - python
  - tools
---

## Nannyml
Is a python package that can estimate performance of your ml model and can be found here.

> NannyML is an open-source python library that allows you to estimate post-deployment model performance (without access to targets), detect data drift, and intelligently link data drift alerts back to changes in model performance. Built for data scientists, NannyML has an easy-to-use interface, interactive visualizations, is completely model-agnostic and currently supports all tabular use cases, classification and regression.

It does something called [Confidence-based Performance Estimation (CBPE)](https://nannyml.readthedocs.io/en/stable/how_it_works/performance_estimation.html#performance-estimation-deep-dive) that can be used to estimate model performance in absence of labels. It can also detect data drift.

## what do I think about it
I did not look to deeply into the CBPE but a package you can plug into your ML pipeline seems great! It seems you still need to build something on top of the results to get alerts. 

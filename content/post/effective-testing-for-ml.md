---
# title for above
title: "Effective Testing for Ml"
date: 2022-11-30T21:15:14+01:00
draft: false
rating: 5
identifyer:
  - url: https://www.jeremyjordan.me/testing-ml/
# full title of resource
link_title: "Effective testing for machine learning systems"
pubDate: "19 Aug 2020"
authors:
  - Jeremy Jordan
difficulties:
  - intermediate
linktypes:
    - blogpost
tags:
    - testing
    - mlops
    - automation
---

## Effective Testing for Ml
Is a blogpost about testing and can be found [at this blog](https://www.jeremyjordan.me/testing-ml/)

Inspired by [checklist paper](https://homes.cs.washington.edu/~marcotcr/acl20_checklist.pdf).

> In this blog post, we'll cover what testing looks like for traditional software development, why testing machine learning systems can be different, and discuss some strategies for writing effective tests for machine learning systems. We'll also clarify the distinction between the closely related roles of evaluation and testing as part of the model development process. By the end of this blog post, I hope you're convinced of both the extra work required to effectively test machine learning systems and the value of doing such work.


    Model evaluation covers metrics and plots which summarize performance on a validation or test dataset.
    Model testing involves explicit checks for behaviors that we expect our model to follow.

## what do I think about it
Describes really well what traditional testing is like and what traditional ML development is like. 

Interesting ideas:
- pre-train tests: identify some bugs early on  during training.  shape of data, output ranges.
- post train tests: done on model artefact. behavioral report of model performance. Things that should not change output, things that should change output. 

I really like this post!

---
# title for above
title: "Problem With Metrics Ml"
date: 2022-11-30T21:55:39+01:00
draft: false
rating: 3
identifyer:
  - doi: https://doi.org/10.48550/arXiv.2002.08512
  - url: https://arxiv.org/ftp/arxiv/papers/2002/2002.08512.pdf
  - arxiv: https://arxiv.org/abs/2002.08512
# full title of resource
link_title: "Reliance on Metrics is a Fundamental Challenge for AI"
pubDate: "20 Feb 2020"
authors:
  - Rachel Thomas
  - David Uminsky
difficulties:
  - intermediate
linktypes:
    - paper
tags:
    - Fairness (in ml)
    - bias
    - guardrail metrics
    - include stakeholders
---

## Reliance on Metrics is a Fundamental Challenge for AI
Is an academic pre-print and can be found [here](https://arxiv.org/abs/2002.08512).

> Optimizing a given metric is a central aspect of most current AI approaches, yet overemphasizing metrics leads to manipulation, gaming, a myopic focus on short-term goals, and other unexpected negative consequences. This poses a fundamental challenge in the use and development of AI. We first review how metrics can go wrong in practice and aspects of how our online environment and current business practices are exacerbating these failures. We put forward here an evidence based framework that takes steps toward mitigating the harms caused by overemphasis of metrics within AI by: (1) using a slate of metrics to get a fuller and more nuanced picture, (2) combining metrics with qualitative accounts, and (3) involving a range of stakeholders, including those who will be most impacted.

> We find from this review the following well supported principles:
-  Any metric is just a proxy for what you really care about
-  Metrics can, and will, be gamed
-  Metrics tend to overemphasize short-term concerns
-  Many online metrics are gathered in highly addictive environments


> We conclude by proposing a framework for the healthier use of metrics that includes:
-  Use a slate of metrics to get a fuller picture
-  Combine metrics with qualitative accounts
-  Involve a range of stakeholders, including those who will be most impacted


## what do I think about it
This is yet another example of applying ML without thinking about your data gives bad results.
But it is not ML specific, although ML makes it easier to apply unfairness at scale, examples of teaching for the test when standardized scores became important. 

Their recommondation of a 'slate of metrics' matches the idea of guardrail metrics: measuring your impact on things that should not change: if the clickthrough rate increases, the percentage of actual purchases should stay the same or also increase. These are sanity checks you should always add to your system.  

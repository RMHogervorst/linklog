---
# title for above
title: "Kumara2022 Mlops Reference Architecture"
date: 2022-11-23T18:33:49+01:00
draft: false
rating: 
identifyer:
  - url: https://www.techrxiv.org/articles/preprint/Requirements_and_Reference_Architecture_for_MLOps_Insights_from_Industry/21397413
  - DOI: 10.36227/techrxiv.21397413.v1
# full title of resource
link_title: "Requirements and Reference Architecture for MLOps:Insights from Industry"
authors: 
  - Indika Kumara 
  - Rowan Arts
  - Dario Di Nucci
  - Willem Jan Van Den Heuvel
  - Damian Andrew Tamburri
difficulties:
  - advanced
linktypes:
    - paper
tags:
    - mlops
    - ml design
    - model serving
    - automation
    - ci/cd
    - training pipelines
    - deployment pipelines
    - monitoring
    - versioning
---

## Kumara2022 Mlops Reference Architecture
[Kumara et al.](https://www.techrxiv.org/articles/preprint/Requirements_and_Reference_Architecture_for_MLOps_Insights_from_Industry/21397413) looked into the 'grey' literature what companies are saying they are using right now. 


Abstract:

> Machine Learning Operations (MLOps) streamline the lifecycle of machine-learning models in production. In recent years, the topic has picked the interest of practitioners, and consequently, a considerable number of tools and gray literature on architecting MLOps environments has emerged. However, this has created a new problem for organizations: selecting the most appropriate tools and design options for implementing their MLOps environments. To alleviate this problem, this paper proposes a reference architecture and requirements for MLOps by systematically reviewing 58 industrial gray literature articles. Such reference architecture drawn from the state of practice shall aid organizations in making better design and technology choices when embarking on their MLOps journey while providing a technology-independent baseline for further MLOps research. 


Damn: 

> We identified 257 sources and applied inclusion/exclusion criteria and quality assessment criteria to create a final list of 58 literature sources.

![layered reference architecture image from paper](/img/kumara_2022_ref_architecture_mlops.png)

![and an overview of different pipelines](kumara2022_pipelines.png)

## what do I think about it
This is very thorough and a bit too much for me. I don't see people setting this up in one go. 
I'd like a minimal version of this. 
This is a short paper with many components. I have to do a deepdive in this paper in the future.
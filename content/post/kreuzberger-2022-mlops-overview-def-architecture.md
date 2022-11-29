---
# title for above
title: "Kreuzberger 2022 Mlops Overview Def Architecture"
date: 2022-11-28T10:39:52+01:00
draft: false
rating: 3
identifyer:
  - arxiv: https://arxiv.org/abs/2205.02302
  - url: https://arxiv.org/ftp/arxiv/papers/2205/2205.02302.pdf
  - DOI: https://doi.org/10.48550/arXiv.2205.02302
# full title of resource
link_title: "Machine Learning Operations (MLOps): Overview, Definition, and Architecture"
authors:
  - Dominik Kreuzberger
  - Niklas Kühl
  - Sebastian Hirschl
difficulties:
  - advanced
linktypes:
    - paper
tags:
  - mlops
  - fundamentals
  - data versioning
  - model versioning
  - code versioning
  - orchestration 
  - training pipelines
  - continuous training (CT)
  - feature engineering pipelines
  - monitoring
  - DevOps
  - CI/CD
  - production
---

## Machine Learning Operations (MLOps): Overview, Definition, and Architecture
Is a unofficial IBM publication and can be found at [arxiv](https://arxiv.org/abs/2205.02302). 
They looked at literature, tools and interviews


> The final goal of all industrial machine learning (ML) projects is to develop ML products and rapidly bring them into production. However, it is highly challenging to automate and operationalize ML products and thus many ML endeavors fail to deliver on their expectations. The paradigm of Machine Learning Operations (MLOps) addresses this issue. MLOps includes several aspects, such as best practices, sets of concepts, and development culture. However, MLOps is still a vague term and its consequences for researchers and professionals are ambiguous. To address this gap, we conduct mixed-method research, including a literature review, a tool review, and expert interviews. As a result of these investigations, we provide an aggregated overview of the necessary principles, components, and roles, as well as the associated architecture and workflows. Furthermore, we furnish a definition of MLOps and highlight open challenges in the field. Finally, this work provides guidance for ML researchers and practitioners who want to automate and operate their ML products with a designated set of technologies. 


They find 9 principles:
- CI/CD automation
- workflow orchestration
- reproducibility
- versioning
- collaboration
- continuous ML training and evaluation
- ML metadata tracking/logging
- continous monitoring
- feedback loops

This (sort of) leads to engineering components:
- CI/CD
- Source code repository
- Workflow orchestration
- Feature store
- Model training infrastructure
- Model registry
- ML metadata stores
- Model serving component
- Monitoring component

and requires a set of roles
- business stakeholder (similar roles: Product Owner,Project Manager)
- solution architect (similar role: IT Architect)
- data scientist (similar roles: ML Specialist, MLDeveloper)
- data engineer (similar role: DataOps Engineer)
- Software engineer
- DevOps engineer
- ML engineer/MLOps engineer

![detail image (venn diagram) from this paper about roles, they overlap quite a bit with mlengineer in the middle](/img/kruezberger2022mlopsroles.png)


### Architecture
![a very complex diagram depicting the entire mlops architecture](/img/kreuzberger2022mlops-architecture.png)

## what do I think about it

> However, MLOps is still a vague term and its consequences for researchers and professionals are ambiguous. 

Boy do they get that right! 

It is hard to distinguish MLOps from devOps, maybe it is just a special flavour or devOps?
What is the difference between principle 6 'continous evalution' and principle 8 'continous monitoring'?

In the architecture diagram I like the different zones:
- MLOps Project Initiation Zone
- Data Engineering Zone
- ML Experimentation Zone
- ML Production Zone

and the roles that are part of that zone. I think maybe putting this all into 1 diagram makes it super confusing. 
What I like is the 'MLOps project initation' == is it a ML problem and can we make a model
and everything after that is engineering. At Ordina we would call phase A a proof of concept and phase C 'experimenting' we call a prototype and D we would call a product.
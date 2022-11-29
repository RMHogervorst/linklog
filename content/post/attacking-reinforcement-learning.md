---
# title for above
title: "Attacking Reinforcement Learning"
date: 2022-11-28T08:34:02+01:00
draft: false
rating: 3
identifyer:
  - url: https://deepai.org/publication/adversarial-policies-attacking-deep-reinforcement-learning
  - arxiv: https://arxiv.org/pdf/1905.10615v1.pdf
# full title of resource
link_title: "Adversarial Policies: Attacking Deep Reinforcement Learning"
authors:
  - Adam Gleave 
  - Michael Dennis 
  - Neel Kant 
  - Cody Wild 
  - Sergey Levine 
  - Stuart Russell
difficulties:
  - advanced
linktypes:
    - paper
tags:
    - reinforcement attacks
    - adversarial policies
    - reinforcement learning
    - fundamentals
---

## Adversarial Policies: Attacking Deep Reinforcement Learning

Can be found [on the deepAI website](https://deepai.org/publication/adversarial-policies-attacking-deep-reinforcement-learning)

Abstract:

> Deep reinforcement learning (RL) policies are known to be vulnerable to ad-
versarial perturbations to their observations, similar to adversarial examples for
classifiers. However, an attacker is not usually able to directly modify another
agent’s observations. This might lead one to wonder: is it possible to attack
an RL agent simply by choosing an adversarial policy acting in a multi-agent
environment so as to create natural observations that are adversarial? We demon-
strate the existence of adversarial policies in zero-sum games between simulated
humanoid robots with proprioceptive observations, against state-of-the-art vic-
tims trained via self-play to be robust to opponents. The adversarial policies
reliably win against the victims but generate seemingly random and uncoordinated
behavior. We find that these policies are more successful in high-dimensional
environments, and induce substantially different activations in the victim policy net-
work than when the victim plays against a normal opponent. Videos are available
at https://adversarialpolicies.github.io/.



> [...] the adversary wins by taking actions that indirectly cause natural observations that are adversarial for the victim.

## what do I think about it
This seems like a fundamental paper for attacking agents trained with (deep) reinforcement learning. 

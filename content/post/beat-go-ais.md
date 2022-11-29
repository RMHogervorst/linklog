---
# title for above
title: "Beat Go Ais"
date: 2022-11-28T08:24:31+01:00
draft: false
rating: 3
identifyer:
  - arxiv: https://arxiv.org/abs/2211.00241
  - DOI: https://doi.org/10.48550/arXiv.2211.00241
# full title of resource
link_title: "Adversarial Policies Beat Professional-Level Go AIs"
authors:
  - Tony Tong Wang
  - Adam Gleave
   -Nora Belrose
  - Tom Tseng
  - Joseph Miller
  - Michael D Dennis
  - Yawen Duan
  - Viktor Pogrebniak
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
---

## Adversarial Policies Beat Professional-Level Go AIs
ML systems can be be broken in interesting ways. This is a system that is easily beaten by actual humans but will win many times against the current state of the art system. (Builds on ['Adversarial Policies: Attacking Deep Reinforcement Learning'](/post/attacking-reinforcement-learning.html "Adversarial Policies: Attacking Deep Reinforcement Learning A paper by deepAI"))


> We attack the state-of-the-art Go-playing AI system, KataGo, by training an adversarial policy that plays against a frozen KataGo victim. Our attack achieves a >99% win-rate against KataGo without search, and a >50% win-rate when KataGo uses enough search to be near-superhuman. To the best of our knowledge, this is the first successful end-to-end attack against a Go AI playing at the level of a top human professional. Notably, the adversary does not win by learning to play Go better than KataGo -- in fact, the adversary is easily beaten by human amateurs. Instead, the adversary wins by tricking KataGo into ending the game prematurely at a point that is favorable to the adversary. Our results demonstrate that even professional-level AI systems may harbor surprising failure modes.

See <https://goattack.alignmentfund.org/> for example games.

> This paper has demonstrated that even agents at the level of top human professionals can be vulner-
able to adversarial policies. However, our results do not establish how common such vulnerabilities
are. It is possible that KataGo is unusually vulnerable, although this seems unlikely as it is the
strongest publicly-available Go AI system and uses a similar training process to other systems.

## what do I think about it
Superhuman performance on a game with reinforcement learning is (again) not the same as human performance, they just have an amazing long history, not intelligence. And so they fail in a different way. 
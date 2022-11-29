---
# title for above
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: false
rating: 1
identifyer:
  - isbn/doi
  - url
RSS:
  - url: enclosure url (media file)
  - length: enclosure length
  - duration: itunes duration
  - image: often itunes:image
  - title: title
  - link: link
# full title of resource
link_title: ""
pubDate: []
authors: []
difficulties:
  - beginner
  - intermediate
  - advanced
linktypes:
    - paper
    - website
    - blogpost
    - bookchapter
    - presentation
    - conference talk
    - book
    - bookseries
    - course
    - course series
    - podcastepisode
tags:
    - ""
---

## {{ replace .Name "-" " " | title }}
Is a ... and can be found here


## what do I think about it


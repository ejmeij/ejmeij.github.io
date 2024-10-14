---
layout: default
title: "The University of Amsterdam at TREC 2012"
date: "2012-11-09"
categories:
  - "blog"
  - "publication"
  - "unrefereed"
tags:
  - "context-based-entity-linking-university-of-amsterdam-at-tac-2012"
  - "edgar_meij"
  - "edgar-de-meij"
  - "edgar-meij"
  - "entity-linking"
  - "entity-linking-and-retrieval"
  - "information-retrieval"
  - "language-modeling"
  - "machine-learning"
  - "meij-2012-entities"
  - "microblogs"
  - "personalized-time-aware-tweets-summarization"
  - "semantic-linking"
  - "text-mining"
  - "trec-kba"
  - "trec-microblog"
  - "trec-2012-twitter"
  - "trec2012contextresults"
  - "twitter"
  - "york-university-trec-2012"
coverImage: "trec-knowledge-base-acceleration-logo-thumb-90.png"
---

This year the Information and Language Processing Systems (ILPS) group of the University of Amsterdam participated in the Microblog and the Knowledge Base Acceleration (KBA) tracks. <!--more-->In this paper, we describe our participation for each of these tracks, in two largely independent sections. We detail the runs we submitted, present the results of the submitted runs, and, where possible, provide an initial analysis of these results.

As to TREC KBA, this year's single task concerned entity linking on a stream of data. That is, given a target entity from a knowledge base and an incoming stream consisting of textual content such as web pages, news items, and social media content, generate a score for each item based on how pertinent it is to the target entity. Recent advances have enabled a precise manner of analysis, where phrases occurring in documents are automatically linked to entries in a knowledge base. This process is commonly known as entity linking. Entity linking facilitates advanced forms of searching and browsing in various domains and contexts. It can be used, for instance, to anchor the textual resources in background knowledge; authors or readers of a piece of text may find entity links to supply useful pointers. Another application can be found in search engines, where it is increasingly common to link queries to entities and present entity-specific overviews. Typical solutions to entity linking [operate on static collections of documents](http://edgar.meij.pro/adding-semantics-microblogs/ "Adding Semantics to Microblog Posts"). In this year's TREC participation, we adapt our entity linking system to be able to operate in this dynamic setting. To this end, we have implemented an incremental learning algorithm that updates at each time step, thereby improving performance at each point in time. Our algorithm also caters for different levels of aboutness.

\[bibtex key=TREC:2012:wn\]

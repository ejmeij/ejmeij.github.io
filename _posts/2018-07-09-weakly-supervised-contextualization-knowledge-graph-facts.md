---
layout: default
title: "Weakly-supervised Contextualization of Knowledge Graph Facts"
date: "2018-07-09"
categories:
  - "blog"
  - "conference"
  - "publication"
tags:
  - "artificial-intelligence"
  - "context"
  - "entity-linking"
  - "entity-linking-and-retrieval"
  - "fact"
  - "freebase"
  - "knowledge-graph"
  - "semantic-search"
  - "text-mining"
  - "weakly-supervised-contextualization-of-knowledge-graph-facts"
coverImage: "sigir2018.jpg"
---

Knowledge graphs (KGs) model facts about the world; they consist of nodes (entities such as companies and people) that are connected by edges (relations such as founderOf ). Facts encoded in KGs are frequently used by search applications to augment result pages. When presenting a KG fact to the user, providing other facts that are pertinent to that main fact can enrich the user experience and support exploratory information needs. _KG fact contextualization_ is the task of augmenting a given KG fact with additional and useful KG facts. The task is challenging because of the large size of KGs; discovering other relevant facts even in a small neighborhood of the given fact results in an enormous amount of candidates. We introduce a neural fact contextualization method (_NFCM_) to address the KG fact contextualization task. NFCM first generates a set of candidate facts in the neighborhood of a given fact and then ranks the candidate facts using a supervised learning to rank model. The ranking model combines features that we automatically learn from data and that represent the query-candidate facts with a set of hand-crafted features we devised or adjusted for this task. In order to obtain the annotations required to train the learning to rank model at scale, we generate training data automatically using distant supervision on a large entity-tagged text corpus. We show that ranking functions learned on this data are effective at contextualizing KG facts. Evaluation using human assessors shows that it significantly outperforms several competitive baselines.

\[bibtex key=SIGIR:2018:Voskarides\]

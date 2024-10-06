---
title: "Improving the Utility of Knowledge Graph Embeddings with Calibration"
date: "2020-04-02"
categories: 
  - "blog"
  - "in-progress"
  - "publication"
tags: 
  - "calibration"
  - "kbp"
  - "knowledge-base-population"
  - "knowledge-graph"
---

This paper addresses machine learning models that embed knowledge graph entities and relationships toward the goal of predicting unseen triples, which is an important task because most knowledge graphs are by nature incomplete. We posit that while offline link prediction accuracy using embeddings has been steadily improving on benchmark datasets, such embedding models have limited practical utility in real-world knowledge graph completion tasks because it is not clear when their predictions should be accepted or trusted. To this end, we propose to calibrate knowledge graph embedding models to output reliable confidence estimates for predicted triples. In crowdsourcing experiments, we demonstrate that calibrated confidence scores can make knowledge graph embeddings more useful to practitioners and data annotators in knowledge graph completion tasks. We also release two resources from our evaluation tasks: An enriched version of the FB15K benchmark and a new knowledge graph dataset extracted from Wikidata.

\[bibtex key=ARXIV:2020:Safavi\]

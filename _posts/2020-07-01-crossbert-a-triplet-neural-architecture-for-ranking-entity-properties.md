---
layout: default
title: "CrossBERT: A Triplet Neural Architecture for Ranking Entity Properties"
date: "2020-07-01"
categories:
  - "blog"
  - "conference"
  - "publication"
coverImage: "SIGIR2020_logo_200-e1614421431991.png"
---

Task-based Virtual Personal Assistants (VPAs) such as the Google Assistant, Alexa, and Siri are increasingly being adopted for a wide variety of tasks. These tasks are grounded in real-world entities and actions (e.g., book a hotel, organise a conference, or requesting funds). In this work we tackle the task of automatically constructing actionable knowledge graphs in response to a user query in order to support a wider variety of increasingly complex assistant tasks. We frame this as an entity property ranking task given a user query with annotated properties. We propose a new method for property ranking, CrossBERT. CrossBERT builds on the Bidirectional Encoder Representations from Transformers (BERT) and creates a new triplet network structure on cross query-property pairs that is used to rank properties. We also study the impact of using external evidence for query entities from textual entity descriptions. We perform experiments on two standard benchmark collections, the NTCIR-13 Actionable Knowledge Graph Generation (AKGG) task and Entity Property Identification (EPI) task. The results demonstrate that CrossBERT significantly outperforms the best performing runs from AKGG and EPI, as well as previous state-of-the-art BERT-based models. In particular, CrossBERT significantly improves Recall and NDCG by approximately 2-12% over the BERT models across the two used datasets. \[\[bibtex key=SIGIR:2020:Manotumruksa\]

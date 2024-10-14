---
layout: default
title: "Expanding Queries Using Multiple Resources"
date: "2007-01-12"
categories:
  - "publication"
  - "unrefereed"
tags:
  - "content"
  - "edgar-lemur"
  - "expanded-search-query-genomics"
  - "indri"
  - "information-retrieval"
  - "lemur"
  - "lucene"
  - "mail-aida-development-de"
  - "mail-aida-development-de-locus"
  - "mesh"
  - "search-query-expansion-multiple-sentences"
  - "semantic-search-indri"
  - "semanticsearchindri"
  - "trac-genomics-meij-jansen"
  - "trec-genomics"
coverImage: "paper_3.png"
---

We describe our participation in the TREC 2006 Genomics track, in which our main focus was on query expansion. We hypothesized that applying query expansion techniques would help us both to identify and retrieve synonymous terms, and to cope with ambiguity. To this end, we developed several collection-specific as well as web-based strategies. We also performed post-submission experiments, in which we compare various retrieval engines, such as Lucene, Indri, and Lemur, using a simple baseline topic set. When indexing entire paragraphs as pseudo-documents, we find that Lemur is able to achieve the highest document-, passage-, and aspect-level scores, using the KL-divergence method and its default settings. Additionally, we index the collection at a lower level of granularity, by creating pseudo-documents comprising of individual sentences. When we search these instead of paragraphs in Lucene, the passage-level scores improve considerably. Finally we note that stemming improves overall scores by at least 10%.

\[bibtex key=TREC:2006:meij\]

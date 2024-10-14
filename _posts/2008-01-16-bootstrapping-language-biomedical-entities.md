---
layout: default
title: "Bootstrapping Language Associated with Biomedical Entities"
date: "2008-01-16"
categories:
  - "publication"
  - "unrefereed"
tags:
  - "bootstrapping-language-model"
  - "entity-trec-entity-prior"
  - "information-extraction"
  - "information-retrieval"
  - "language-modeling"
  - "query-modeling"
  - "semantic-query-analysis"
  - "trec-genomics"
coverImage: "text_mining340x220.png"
---

The TREC Genomics 2007 task included recognizing topic-specific entities in the returned passages. To address this task, we have designed and implemented a novel data-driven ap- proach by combining information extraction with language modeling techniques. Instead of using an exhaustive list of all possible instances for an entity type, we look at the language usage around each entity type and use that as a classifier to determine whether or not a piece of text discusses such an entity type. We do so by comparing it with language models of the passages. E.g., given the entity type “genes”, our approach can measure the gene-iness of a piece of text.

Our algorithm works as follows. Given an entity type, it first uses Hearst patterns to extract instances of the type. To extract more instances, we look for new contextual patterns around the instances and use them as input for a bootstrapping method, in which new instances and patterns are discovered iteratively. Afterwards, all discovered instances and patterns are used to find the sentences in the collection which are most on par with the requested entity type. A language model is then generated from these sentences and, at retrieval time, we use this model to rerank retrieved passages.

As to the results of our submitted runs, we find that our baseline run performs well above the median of all participant’s scores. Additionally, we find that applying our proposed method helps the entity types for which there are unambiguous patterns and numerous instances most.

\[bibtex key=TREC:2008:meij\]

http://www.slideshare.net/edgar.meij/trec-2007-genomics-talk-edgar-meij-univ-of-amsterdam-presentation/

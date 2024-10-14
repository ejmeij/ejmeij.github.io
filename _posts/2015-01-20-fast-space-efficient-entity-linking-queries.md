---
layout: default
title: "Fast and Space-Efficient Entity Linking in Queries"
date: "2015-01-20"
categories:
  - "blog"
  - "conference"
  - "publication"
tags:
  - "compression"
  - "entity-linking"
  - "fast-and-space-efficient-entity-linking-in-queries"
  - "httpedgar-meij-profast-space-efficient-entity-linking-queriesutm_sourcebit-ly"
  - "information-retrieval"
  - "me-ij"
  - "meij"
  - "web-search"
  - "wikipedia"
coverImage: "wsdm_2015.png"
---

Entity linking deals with identifying entities from a knowledge base in a given piece of text and has become a fundamental building block for web search engines, enabling numerous downstream improvements from better document ranking to enhanced search results pages. A key problem in the context of web search queries is that this process needs to run under severe time constraints as it has to be performed before any actual retrieval takes place, typically within milliseconds. In this paper we propose a probabilistic model that leverages user-generated information on the web to link queries to entities in a knowledge base. There are three key ingredients that make the algorithm fast and space-efficient. First, the linking process ignores any dependencies between the different entity candidates, which allows for a O(k^2) implementation in the number of query terms. Second, we leverage hashing and compression techniques to reduce the memory footprint. Finally, to equip the algorithm with contextual knowledge without sacrificing speed, we factor the distance between distributional semantics of the query words and entities into the model. We show that our solution significantly outperforms several state-of-the-art baselines by more than 14% while being able to process queries in sub-millisecond times—at least two orders of magnitude faster than existing systems.

\[bibtex key=WSDM:2015:blanco\]

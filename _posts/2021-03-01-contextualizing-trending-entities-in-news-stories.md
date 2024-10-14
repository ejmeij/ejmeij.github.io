---
layout: default
title: "Contextualizing Trending Entities in News Stories"
date: "2021-03-01"
categories:
  - "blog"
  - "conference"
  - "publication"
tags:
  - "information-retrieval"
  - "learning-to-rank"
  - "trend-detection"
coverImage: "wsdm.png"
---

Trends are those keywords, phrases, or names that are mentioned most often on social media or in news in a particular timeframe.They are an effective way for human news readers to both discover and stay focused on the most relevant information of the day. In this work, we consider trends that correspond to an entity in a knowledge graph and introduce the new and as-yet unexplored task of identifying other entities that may help explain the "why" an entity is trending. We refer to these retrieved entities as contextual entities. Some of them are more important than others in the context of the trending entity and we thus determine a ranking of entities according to how useful they are in contextualizing the trend. We propose two solutions for ranking contextual entities. The first one is fully unsupervised and based on Personalized PageRank, calculated over a trending entity-specific graph of other entities where the edges encode a notion of directional similarity based on embedded background knowledge. Our second method is based on learning to rank and combines the intuitions behind the unsupervised model with signals derived from hand-crafted features in a supervised setting. We compare our models on this novel task by using a new, purpose-built test collection created using crowdsourcing. Our methods improve over the strongest baseline in terms of Precision at 1 by 7% (unsupervised) and 13% (supervised). We find that the salience of a contextual entity and how coherent it is with respect to the news story are strong indicators of relevance in both unsupervised and supervised settings.

See [https://doi.org/10.1145/3437963.3441765](https://doi.org/10.1145/3437963.3441765).

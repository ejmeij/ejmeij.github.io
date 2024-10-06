---
title: "Mapping queries to the Linking Open Data cloud: A case study using DBpedia"
date: "2011-04-02"
categories:
  - "journal"
  - "publication"
tags:
  - "compare-data-clouds"
  - "concept-vector-dbpedia"
  - "dbpedia"
  - "edgar-meij-linked-open-data"
  - "entity-linking"
  - "information-retrieval"
  - "linked-open-data-case-study"
  - "linked-open-data-data-mining"
  - "linked-open-data-text-mining"
  - "linking-open-data"
  - "lod"
  - "machine-learning"
  - "mapping-queries-to-the-linking-open-data-cloud-a-case-study-using-dbpedia"
  - "mapping-queries-to-the-linking-open-data-cloud-a-case-study-using-dbpedia-download"
  - "query"
  - "query-linked-open-data"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semantic-search"
  - "semanticizing"
  - "supervised-data-mining-on-linked-open-data"
coverImage: "DBpedia.png"
---

We introduce the task of mapping search engine queries to DBpedia, a major linking hub in the Linking Open Data cloud. We propose and compare various methods for addressing this task, using a mixture of information retrieval and machine learning techniques. Specifically, we present a supervised machine learning-based method to determine which concepts are intended by a user issuing a query. The concepts are obtained from an ontology and may be used to provide contextual information, related concepts, or navigational suggestions to the user submitting the query. Our approach first ranks candidate concepts using a language modeling for information retrieval framework. We then extract query, concept, and search-history feature vectors for these concepts. Using manual annotations we inform a machine learning algorithm that learns how to select concepts from the candidates given an input query. Simply performing a lexical match between the queries and concepts is found to perform poorly and so does using retrieval alone, i.e., omitting the concept selection stage. Our proposed method significantly improves upon these baselines and we find that support vector machines are able to achieve the best performance out of the machine learning algorithms evaluated.

\[bibtex key=JWS:2011:meij\]

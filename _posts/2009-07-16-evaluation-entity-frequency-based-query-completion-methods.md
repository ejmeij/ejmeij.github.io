---
layout: default
title: "An evaluation of entity and frequency based query completion methods"
date: "2009-07-16"
categories:
  - "conference"
  - "publication"
tags:
  - "an-evaluation-of-entity-and-frequency-based-query-completion-methods"
  - "contextualizationsearchwikipediaconcept"
  - "dbpedia"
  - "digital-camera-and-frequencies-of-entities"
  - "entity-based-query-log"
  - "information-retrieval-dbpedia"
  - "information-retrieval-with-dbpedia"
  - "mining-dbpedia"
  - "o-meij-bool"
  - "query-log-analysis"
  - "retrieval-dbpedia"
  - "semantic-query-analysis"
  - "semantic-search"
  - "text-mining-dbpedia"
coverImage: "Untitled.png"
---

From the days of boolean search on library catalogues, users have reformulated their queries after an inspection of initial search results. Traditional information retrieval studies this in frameworks such as query expansion, relevance feedback, interactive retrieval, etc. These methods mostly exploit document contents because that is typically all information that is available. The situation is very different in web search engines because of the large amounts of users whose queries are collected in query logs. Query logs reflect how large numbers of users express their queries and can be a rich source of information when optimizing search results or determining query suggestions.

In this paper we study a special case of query suggestion: query completion, which aims to help users complete their queries. In particular, we are interested in comparing a commonly adopted frequency-based approach with methods that exploit an understanding of the type of entities in queries. Our intuition is that completion for rare queries can be improved by understanding the type of entity being sought. For example, if we know that “LX354” is a kind of digital camera, we can generate sensible completions by choosing them from the set of completions used with other digital cameras. Besides suggesting queries, the obtained completions can also function as facets for faceted browsing or as input for ontology engineering since they represent query refinements common to a class of entities. In this paper, we address the following questions: (i) How can we recognize entities and their types in queries? (ii) How can we rank possible completions given an entity type? (iii) How can our methods be evaluated and how do they perform? To address (iii), we propose a novel method which evaluates the prediction of real web queries. We show that a purely frequency-based approach without any entity type information works quite well for more frequent queries, but is surpassed by type-based methods for rare queries.

\[bibtex key=SIGIR:2009:meij\]

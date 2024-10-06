---
title: "Linking queries to entities"
date: "2014-02-24"
categories: 
  - "blog"
tags: 
  - "entity-linking"
  - "entity-linking-bio-energy"
  - "entity-linking-query-yahoo"
  - "entity-segmentation-in-entity-disambiguous"
  - "httpedgar-meij-prolinking-queries-entities"
  - "httpedgr"
  - "httpsedgar-meij-prolinking-queries-entities"
  - "linking-labs-to-panytopenia-for-queries"
  - "linking-queries-to-entities"
  - "other-name-of-panytopenia"
  - "query-log-analysis"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semantic-search"
  - "semanticizing"
  - "text-mining"
  - "wikipedia"
  - "yahoo-query-entity-linking"
coverImage: "5653ceb29b32c4e3b18d84170b6b707e.jpeg"
---

I'm happy to announce we're releasing a new test collection for entity linking for web queries (within user sessions) to Wikipedia. About half of the queries in this dataset are sampled from Yahoo search logs, the other half comes from the TREC Session track. Check out [the L24 dataset](http://webscope.sandbox.yahoo.com/catalog.php?datatype=l "http://webscope.sandbox.yahoo.com/catalog.php?datatype=l") on [Yahoo Webscope](http://yahooresearch.tumblr.com/post/77697901734/welcome-to-webscope "Welcome to Webscope"), or drop me a line for more information. Below you'll find an excerpt of the README text associated with it.

With this dataset you can train, test, and benchmark entity linking systems on the task of linking web search queries – within the context of a search session – to entities. Entities are a key enabling component for semantic search, as many information needs can be answered by returning a list of entities, their properties, and/or their relations. A first step in any such scenario is to determine which entities appear in a query – a process commonly referred to as named entity resolution, named entity disambiguation, or semantic linking.

This dataset allows researchers and other practitioners to evaluate their systems for linking web search engine queries to entities. The dataset contains manually identified links to entities in the form of Wikipedia articles and provides the means to train, test, and benchmark such systems using manually created, gold standard data. With releasing this dataset publicly, we aim to foster research into entity linking systems for web search queries. To this end, we also include sessions and queries from the TREC Session track (years 2010–2013). Moreover, since the linked entities are aligned with a specific part of each query (a "span"), this data can also be used to evaluate systems that identify spans in queries, i.e, that perform query segmentation for web search queries, in the context of search sessions.

The key properties of the dataset are as follows.

- Queries are taken from Yahoo US Web Search and from the TREC Session track (2010-2013).
- There are 2635 queries in 980 sessions, 7482 spans, and 5964 links to Wikipedia articles in this dataset.
- The annotations include the part of the query (the "span") that is linked to each Wikipedia article. This information can also be used for query segmentation experiments.
- The annotators have identified the "main" entity/ies for each query, if available.
- The annotators also labeled the queries, identifying whether they are non-English, navigational, quote-or-question, adult, or ambiguous and also if an out-of-Wikipedia entity is mentioned in the query, i.e., when an entity is mentioned in a query but no suitable Wikipedia article exists.
- The file includes session information: each session consists of an anonymized id, initial query, as well as all the queries issued within the same session and their relative date/timestamp if available.
- Sessions are demarcated using a 30 minute time-out.

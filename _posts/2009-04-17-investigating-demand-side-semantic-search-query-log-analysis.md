---
title: "Investigating the Demand Side of Semantic Search through Query Log Analysis"
date: "2009-04-17"
categories: 
  - "publication"
  - "workshop"
tags: 
  - "ad-hoc-log-analysis"
  - "dbpedia"
  - "dbpedia-machine-learning"
  - "dbpedia-query-log"
  - "how-to-get-query-log-for-information-retrieval"
  - "how-to-get-querylog"
  - "information-retrieval-log-analysis"
  - "machine-learning-dbpedia"
  - "publishing-search-logs"
  - "query-log-analysis"
  - "semantic-query-analysis"
  - "semantic-search"
  - "semantic-analysis-using-dbpedia"
  - "semantic-enrichment"
  - "semantic-search-information-retrieval"
  - "semantic-search-log-analysis"
  - "semantic-search-query-analysis"
  - "twitter-query-log"
  - "twitter-query-log-analyzer"
  - "twitterloganalyze"
coverImage: "crowd.jpg"
---

Semantic search is by its broadest definition a collection of approaches that aim at matching the Web’s content with the information need of Web users at a semantic level. Most of the work in this area has focused on the supply-side of semantic search, in particular elevating Web content to the semantic level by relying on methods of information extraction or working with explicit metadata embedded inside or linked to Web resources. With respect to explicit metadata, several studies have been done on the adoption of semantic web formats in the wild, mostly based on statistics from the crawls of semantic web search engines. Much less effort has focused on the demand-side of semantic search, i.e. interpreting queries at the semantic level and studying information needs at this level. Conversely, little is known as to how much the supply of metadata actually matches the demand for information on the Web.

In this paper, we address the problem of studying the information need of Web searchers at an ontological level, i.e., in terms of the particular attributes of objects they are interested in. We describe a set of methods for extracting the context words to certain classes of objects from a Web search query log. We do so based on the idea that common context words reflects aspects of objects users are interested in. We implement these methods in an interactive tool called the Semantic Search Assist. The original purpose of this tool was to generate type-based query suggestions when there is not enough statistical evidence for entity-based query suggestions. However, from an ontology engineering perspective, this tool answers the question of what attributes a class of objects would have if the ontology for it was engineered purely based on the information needs of end users. As such it allows us to reflect on the gap between the properties defined in Semantic Web ontologies and the attributes of objects that people are searching for on the Web. We evaluate our tool by measuring it’s predictive power on the query log itself. We leave the study of the gap between particular information needs and Semantic Web data for future work.

\[bibtex key=semsearch:2009:meij\]

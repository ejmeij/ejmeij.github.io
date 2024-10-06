---
title: "Parsimonious concept modeling"
date: "2008-07-16"
categories: 
  - "conference"
  - "publication"
tags: 
  - "information-retrieval"
  - "language-modeling"
  - "mesh"
  - "query-modeling"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semantic-search"
  - "trec-genomics"
coverImage: "iStock_000005085186Medium.jpg"
---

In many collections, documents are annotated using concepts from a structured knowledge source such as an ontology or thesaurus. Examples include the news domain, where each news item is categorized according to the nature of the event that took place, and Wikipedia, with its per-article categories. These categorizing systems originally stem from the cataloging systems used in libraries and conceptual search is commonly used in digital library environments at the front-end to support search and navigation. In this paper we want to employ the explicit knowledge used for annotation at the back-end, not just to improve retrieval performance, but also to generate high-quality term and concept suggestions. To do so, we use the dual document representation— concepts and terms—to create a generative language model for each concept, which bridges the gap between vocabulary terms and concepts. Related work has also used textual representations to rep- resent concepts, however, there are two important differences. First, we use statistical language modeling techniques to parametrize the concept models, by leveraging the dual represen- tation of the documents. Second, we found that simple maximum likelihood estimation assigns too much probability mass to terms and concepts which may not be relevant to each document. Thus we apply an EM algorithm to “parsimonize” the document models.

The research questions we address are twofold: (i) what are the results of applying our model as compared to a query-likelihood baseline as well as compared to a run based on relevance models and (ii) what is the influence of parsimonizing? To answer these questions, we use the TREC Genomics track test collections in conjunction with MedLine. MedLine contains over 16 million bibliographic records of publications from the life sciences domain and each abstract therein has been manually indexed by trained curators, who use concepts from the MeSH (Medical Subject Headings) thesaurus. We show that our approach is able to achieve similar or better performance than relevance models, whilst at the same time providing high quality concepts to facilitate navigation. Examples show that our parsimonious concept models generate terms that are more specific than those acquired through maximum likelihood estimates.

\[bibtex key=SIGIR:2008:Meij-cm\]

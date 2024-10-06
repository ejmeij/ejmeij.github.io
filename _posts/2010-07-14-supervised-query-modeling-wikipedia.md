---
title: "Supervised query modeling using Wikipedia"
date: "2010-07-14"
categories:
  - "conference"
  - "publication"
tags:
  - "dbpedia"
  - "entity-linking"
  - "information-retrieval"
  - "language-modeling"
  - "linking-open-data"
  - "lod"
  - "machine-learning"
  - "query-modeling"
  - "query-modelling-using"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semantic-search"
  - "sigir-2010-wikipedia"
  - "sigir-vikipediya"
  - "sigir-wikipedia"
  - "supervised-query-modeling-using-wikipedia-in-proceeding-of-the-33rd-international-acm-sigir-conference-on-research-and-development-in-information-retrieval"
coverImage: "Wikipedia.png"
---

In a web retrieval setting, there is a clear need for precision enhancing methods. For example, the query “the secret garden” (a novel that has been adapted into movies and musicals) is a query that is easily led astray because of the generality of the individual query terms. While some methods address this issue at the document level, e.g., by using anchor texts or some function of the web graph, we are interested in improving the query; a prime example of such an approach is leveraging phrasal or proximity information. Besides degrading the user experience, another significant downside of a lack of precision is its negative impact on the effectiveness of pseudo relevance feedback methods. An example of this phenomenon can be observed for a query such as “indexed annuity” where the richness of the financial domain plus the broad commercial use of the web introduces unrelated terms. To address these issues, we propose a semantically informed manner of representing queries that uses supervised machine learning on Wikipedia. We train an SVM that automatically links queries to Wikipedia articles which are subsequently used to update the query model.

Wikipedia and supervised machine learning have previously been used to select optimal terms to include in the query model. We, however, are interested in selecting those Wikipedia articles which best describe the query and use those to sample terms from. This is similar to the unsupervised manner used, e.g., in the context of retrieving blogs. Such approaches are completely unsupervised in that they only consider a fixed number of pseudo relevant Wikipedia articles. As we show, focusing this set using machine learning improves overall retrieval performance. In particular, we apply supervised machine learning to automatically link queries to Wikipedia articles and sample terms from the linked articles to re-estimate the query model. On a recent large web corpus, we observe substantial gains in terms of both traditional metrics and diversity measures.

\[bibtex key=SIGIR:2010:meij\]

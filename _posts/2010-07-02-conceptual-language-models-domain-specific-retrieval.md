---
layout: default
title: "Conceptual language models for domain-specific retrieval"
date: "2010-07-02"
categories:
  - "journal"
  - "publication"
tags:
  - "clef"
  - "information-retrieval"
  - "language-modeling"
  - "meij-journal"
  - "mesh"
  - "meta-language"
  - "query-modeling"
  - "semantic-search"
  - "trec-genomics"
coverImage: "84894874_a70bf5a682.jpg"
---

Over the years, various meta-languages have been used to manually enrich documents with conceptual knowledge of some kind. Examples include keyword assignment to citations or, more recently, tags to websites. In this paper we propose generative concept models as an extension to query modeling within the language modeling framework, which leverages these conceptual annotations to improve retrieval. By means of relevance feedback the original query is translated into a conceptual representation, which is subsequently used to update the query model.

Extensive experimental work on five test collections in two domains shows that our approach gives significant improvements in terms of recall, initial precision and mean average precision with respect to a baseline without relevance feedback. On one test collection, it is also able to outperform a text-based pseudo-relevance feedback approach based on relevance models. On the other test collections it performs similarly to relevance models. Overall, conceptual language models have the added advantage of offering query and browsing suggestions in the form of conceptual annotations. In addition, the internal structure of the meta-language can be exploited to add related terms.

Our contributions are threefold. First, an extensive study is conducted on how to effectively translate a textual query into a conceptual representation. Second, we propose a method for updating a textual query model using the concepts in conceptual representation. Finally, we provide an extensive analysis of when and how this conceptual feedback improves retrieval.

\[bibtex key=IPM:2010:Meij\]

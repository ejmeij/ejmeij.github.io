---
layout: default
title: "A query model based on normalized log-likelihood"
date: "2009-11-19"
categories:
  - "conference"
  - "publication"
tags:
  - "a-query-model-based-on-normalized-log-likelihood"
  - "information-retrieval"
  - "language-modeling"
  - "log-likelihood-information-retrieval"
  - "normalized-likelihood"
  - "normalized-log-likelihood"
  - "query-modeling"
  - "relevance-modeling"
  - "supervised-query-modeling-using-wikipedia"
  - "the-normalized-likelihood-method"
  - "trec-relevance-feedback"
coverImage: "pr.png"
---

A query is usually a brief, sometimes imprecise expression of an underlying information need . Examining how queries can be transformed to equivalent, potentially better queries is a theme of recurring interest to the information retrieval community. Such transformations include expansion of short queries to long queries, paraphrasing queries using an alternative vocabulary, mapping unstructured queries to structured ones, identifying key concepts in verbose queries, etc.

To inform the transformation process, multiple types of information sources have been considered. A recent one is search engine logs for query substitutions . Another recent example is where users complement their traditional keyword query with additional information, such as example documents, tags, images, categories, or their search history . The ultimate source of information for transforming a query, however, is the user, through relevance feedback : given a query and a set of judged documents for that query, how does a system take advantage of the judgments in order to transform the original query and retrieve more documents that will be useful to the user? As demonstrated by the recent launch of a dedicated relevance feedback track at TREC, we still lack the definitive answer to this question.

Let’s consider an example to see what aspects play a role in transforming a query based on judgments for a set of initially retrieved documents. Suppose we have a set of documents which are judged to be relevant to a query. These documents may vary in length and, furthermore, they need not be completely on topic because they may discuss more topics than the ones that are relevant to the query. While the users’ judgments are at the document level, not all of the documents’ sections can be assumed to be equally relevant. Most relevance feedback models that are currently available do not model or capture this phenomenon; instead, they attempt to transform the original query based on the full content of the documents. Clearly this is not ideal and we would like to account for the possibly multi-faceted character of documents. We hypothesize that a relevance feedback model that attempts to capture the topical structure of individual judged documents (“For each judged document, what is important about it?”) as well as of the set of all judged documents (“Which topics are shared by the entire set of judged documents?”) will outperform relevance feedback models that capture only one of these types of information.

We are working in a language modeling (LM) setting and our aim in this paper is to present an LM-based relevance feedback model that uses both types of information—about the topical relevance of a document and about the general topic of the set of relevant documents— to transform the original query. The proposed model uses the whole set of relevance assessments to determine how much each document that has been judged relevant should contribute to the query transformation. We use the TREC relevance feedback track test collection to evaluate our model and compare it to other, established relevance feedback methods. We show that it is able to achieve superior performance over all evaluated models. We answer the following two research questions in this paper. (i) Can we develop a relevance feedback model that uses evidence from both the individual relevant documents and the set of relevant documents as a whole? (ii) Can our new model achieve state-of-the-art results and how do these results compare to related models? When evaluated, we show that our model is able to significantly improve over state-of-art feedback methods.

\[bibtex key=CIKM:2009:Meij\]

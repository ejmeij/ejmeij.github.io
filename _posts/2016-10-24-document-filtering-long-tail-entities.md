---
layout: default
title: "Document Filtering for Long-tail Entities"
date: "2016-10-24"
categories:
  - "blog"
  - "conference"
  - "publication"
tags:
  - "adaptive-filtering"
  - "dbpedia"
  - "entity-linking"
  - "entity-linking-and-retrieval"
  - "logo-penerbit-buku-internasional"
  - "long-tail"
  - "meij-bloomberg"
  - "penerbit-buku-internasional"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "text-mining"
  - "trec-kba"
  - "wikipedia"
coverImage: "cikm16-e1485513137105.png"
---

Filtering relevant documents with respect to entities is an essential task in the context of knowledge base construction and maintenance. It entails processing a time-ordered stream of documents that might be relevant to an entity in order to select only those that contain vital information. State-of-the-art approaches to document filtering for popular entities are entity-dependent: they rely on and are also trained on the specifics of differentiating features for each specific entity. Moreover, these approaches tend to use so-called _extrinsic_ information such as Wikipedia page views and related entities which is typically only available only for popular head entities. Entity-dependent approaches based on such signals are therefore ill-suited as filtering methods for long-tail entities.<!--more-->

In this paper we propose a document filtering method for long-tail entities that is *entity-independent* and thus also generalizes to unseen or rarely seen entities. It is based on intrinsic features, i.e., features that are derived from the documents in which the entities are mentioned. We propose a set of features that capture informativeness, entity-saliency, and timeliness. In particular, we introduce features based on entity aspect similarities, relation patterns, and temporal expressions and combine these with standard features for document filtering.

Experiments following the TREC KBA 2014 setup on a publicly available dataset show that our model is able to improve the filtering performance for long-tail entities over several baselines. Results of applying the model to unseen entities are promising, indicating that the model is able to learn the general characteristics of a vital document. The overall performance across all entities–i.e., not just long-tail entities–improves upon the state-of-the-art without depending on any entity-specific training data.

\[bibtex key=CIKM:2016:Reinanda\]

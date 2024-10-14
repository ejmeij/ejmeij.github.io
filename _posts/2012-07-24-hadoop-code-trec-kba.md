---
layout: default
title: "Hadoop code for TREC KBA"
date: "2012-07-24"
categories:
  - "blog"
tags:
  - "edgar-meij"
  - "edgar-meij-hadoop"
  - "edgar-meij-publications"
  - "ejmeij-on-twitter"
  - "entity-finding"
  - "entity-linking"
  - "entity-search-edgar-tutorial"
  - "hadoop"
  - "hadoop-semantic"
  - "hadoop-semantic-search"
  - "how-to-do-trec-microblog"
  - "java"
  - "java-meij"
  - "replab-2012-dataset"
  - "semantic-linking"
  - "semanticizing"
  - "thrift"
  - "trec-kba"
  - "trec-kba-hadoop"
  - "wikipedia"
coverImage: "trec-knowledge-base-acceleration-logo-thumb-90.png"
---

I've decided to put some of the Hadoop code I developed for the TREC KBA task online. It's available on Github: [https://github.com/ejmeij/trec-kba](https://github.com/ejmeij/trec-kba). In particular, it provides classes to read/write topic files, read/write run files, and expose the documents in the Thrift files as Hadoop-readable objects ('ThriftFileInputFormat') to be used as input to mappers. I obviously also implemented a toy KBA system on Hadoop :-). See Github for more info.

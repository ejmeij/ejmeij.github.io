---
title: "Deploying Lucene on the Grid"
date: "2006-07-01"
categories:
  - "publication"
  - "workshop"
tags:
  - "grid-computing"
  - "gridlucene"
  - "information-retrieval"
  - "lucene"
  - "lucene-ir-grid"
  - "lucene-literature"
  - "lucene-papers"
  - "lucene-pubmed"
  - "lucene-semantic"
  - "lucene-semantic-information"
  - "lucene-semantic-search"
  - "lucene-tag-search"
  - "pubmed-lucene"
  - "semantic-search-application-using-lucene-2011"
  - "semantic-search-lucene"
  - "semantic-search-using-lucene"
  - "semantic-search-using-lucene-abstract"
  - "semantic-search-with-lucene"
  - "semantic-tags-lucene"
  - "sematic-search-with-lucene"
coverImage: "lucene_med.png"
---

We investigate if and how open source retrieval engines can be deployed in a grid environment. When comparing grids to conventional distributed IR, the lack of a-priori knowledge about available nodes is one of the most significant differences. On top of that, it is also unknown when a particular node has time and resources available and starts a submitted job. Therefore, conventional methods such as RMI are not directly usable and we propose a different approach, using middleware designed specifically for grids. We describe GridLucene, an extension of the open source engine Lucene with grid-specific classes, based on this middleware. We report on an initial comparison between GridLucene and Lucene, and find a minor penalty (in terms of execution time) for grid-based indexing and a more serious penalty for grid-based retrieval.

The used middleware can gather a set of physical resources to form a single logical resource with some abstract properties. The user-definable properties can be used during indexing and retrieval to let GridLucene know which files it needs to access. By using this kind of semantic information, grid nodes can “discover” which indices exist on the grid and which particular documents need to be indexed.

GridLucene is available for downloading under the same license as Lucene.

\[bibtex key=OSIR:2005:meij\]

---
layout: default
title: "Team COMMIT at TREC 2011"
date: "2012-01-25"
categories:
  - "publication"
  - "unrefereed"
tags:
  - "entity-linking"
  - "information-retrieval"
  - "lod"
  - "query-modeling"
  - "releasedtrec2011microblog"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semantic-search"
  - "semanticizing"
  - "team-commit"
  - "trec-entity"
  - "trec-microblog"
  - "trec-2011-microblog"
  - "trec-2011-microblog-proceeding"
  - "trec-2011-working-note"
  - "trec-blogs-html-tag-filter-trec-star-trek"
  - "trec-elc-2011-number-of-topics"
  - "trec-entity-track-elc-2011-topics-proceedings"
  - "trec-microblog-overview"
  - "trec2011workingnotes"
  - "university-of-amsterdam-commit-team"
coverImage: "microblogtrarck.png"
---

We describe the participation of Team COMMIT in this year’s Microblog and Entity track.

In our participation in the Microblog track, we used a feature-based approach. Specifically, we pursued a precision oriented recency-aware retrieval approach for tweets. Amongst others we used various types of external data. In particular, we examined the potential of link retrieval on a corpus of crawled content pages and we use semantic query expansion using Wikipedia. We also deployed pre-filtering based on query-dependent and query-independent features. For the Microblog track we found that a simple cut-off based on the z-score is not sufficient: for differently distributed scores, this can decrease recall. A well set cut-off parameter can however significantly increase precision, especially if there are few highly relevant tweets. Filtering based on query-independent filtering does not help for already small result list. With a high occurrence of links in relevant tweets, we found that using link retrieval helps improving precision and recall for highly relevant and relevant tweets. Future work should focus on a score-distribution dependent selection criterion.

In this years Entity track participation we focused on the Entity List Completion (ELC) task. We experimented with a text based and link based approach to retrieve entities in Linked Data (LD). Additionally we experimented with selecting candidate entities from a web corpus. Our intuition is that entities occurring on pages with many of the example entities are more likely to be good candidates than entities that do not. For the Entity track there are no analyses or conclusions to report yet; at the time of writing no evaluation results are available for the Entity track.

\[bibtex key=TREC:2011:commit\]

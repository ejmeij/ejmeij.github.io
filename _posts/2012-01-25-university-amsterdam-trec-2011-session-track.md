---
title: "The University of Amsterdam at the TREC 2011 Session Track"
date: "2012-01-25"
categories: 
  - "publication"
  - "unrefereed"
tags: 
  - "how-to-get-trec-2011-session-track-data-set"
  - "information-retrieval"
  - "learning-to-rank"
  - "linking-hub-data"
  - "lori-buckland"
  - "lori-buckland-nist"
  - "query-modeling"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semanticizing"
  - "session-track-at-trec-2011"
  - "session-trec-2011"
  - "trec-sessions"
  - "trec-2011-session-track-best-system"
  - "trec-2011-session-track-data-set"
  - "trec-2011-web-track-system"
  - "trec-session-track"
  - "trec2011workingnotes"
  - "university-of-amsterdam-edgar-meij"
  - "university-of-amsterdam-trec"
coverImage: "paper_3.png"
---

We describe the participation of the University of Amsterdam's ILPS group in the Session track at TREC 2011.

The stream of interactions created by a user engaging with a search system contains a wealth of information. For retrieval purposes, previous interactions can help inform us about a user's current information need. Building on this intuition, our contribution to this TREC year's session track focuses on session modeling and learning to rank using session information. In this paper, we present and compare three complementary strategies that we designed for improving retrieval for a current query using previous queries and clicked results: probabilistic session modeling, semantic query modeling, and implicit feedback.

In our experiments we examined three complementary strategies for improving retrieval for a current query. Our first strategy, based on probabilistic session modeling, was the best performing strategy.

Our second strategy, based on semantic query modeling, did less well than we expected, likely due to topic drift from excessively aggressive query expansion. We expect that performance of this strategy would improve by limiting the number of terms and/or improving the probability estimates.

With respect to our third strategy, based on learning from feedback, we found that learning weights for linear weighted combinations of features from an external collection can be beneficial, if characteristics of the collection are similar to the current data. Feedback available in the form of user clicks appeared to be less beneficial. Our run learning from implicit feedback did perform substantially lower than a run where weights were learned from an external collection with explicit feedback using the same learning algorithm and set of features.

\[bibtex key=TREC:2011:huurnink\]

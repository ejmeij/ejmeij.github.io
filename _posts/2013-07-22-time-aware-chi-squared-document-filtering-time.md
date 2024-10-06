---
title: "Time-Aware Chi-squared for Document Filtering over Time"
date: "2013-07-22"
categories: 
  - "publication"
  - "workshop"
tags: 
  - "adaptive-filtering"
  - "edgar-meij"
  - "edgar-meij-qa-challenge"
  - "meij"
  - "time-aware-chi-squared-for-document-filtering-over-time"
  - "trec-kba"
---

_To appear at TAIA2013 (a SIGIR 2013 workshop)._

Document filtering over time is widely applied in various tasks such as tracking topics in online news or social media. We consider it a classification task, where topics of interest correspond to classes, and the feature space consists of the words associated to each class. In "streaming" settings the set of words associated with a concept may change. In this paper we employ a multinomial Naive Bayes classifier and perform periodic feature selection to adapt to evolving topics. We propose two ways of employing Pearson's χ2 test for feature selection and demonstrate its benefit on the TREC KBA 2012 data set. By incorporating a time-dependent function in our equations for χ2 we provide an elegant method for applying different weighting schemes. Experiments show improvements of our approach over a non-adaptive baseline.

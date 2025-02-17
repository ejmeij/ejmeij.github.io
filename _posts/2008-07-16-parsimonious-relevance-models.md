---
layout: default
title: "Parsimonious Relevance Models"
date: "2008-07-16"
categories:
  - "conference"
  - "publication"
tags:
  - "bettina-berendt"
  - "dpea-em-parsimony"
  - "language-modeling"
  - "parsimonious-feedback"
  - "parsimonious-relevance-models"
  - "query-modeling"
  - "relevance-modeling"
  - "relevant-parsimonious"
  - "trec-blog"
  - "trec-enterprise"
  - "trec-genomics"
  - "trec-blog-collection"
coverImage: "matematicas1.jpg"
---

Relevance feedback is often applied to better capture a user’s information need. Automatically reformulating queries (or blind relevance feedback) entails looking at the terms in some set of (pseudo-)relevant documents and selecting the most informative ones with respect to the set or the collection. These terms may then be reweighed based on information pertinent to the query or the documents and—in a language modeling setting—be used to estimate a query model, P(t|θQ), i.e., a distribution over terms t for a given query Q.

Not all of the terms obtained using blind relevance feedback are equally informative given the query, even after reweighing. Some may be common terms, whilst others may describe the general domain of interest. We hypothesize that refining the results of blind relevance feedback, using a technique called parsimonious language modeling, will improve retrieval effectiveness. Hiemstra et al. already provide a mechanism for incorporating (parsimonious) blind relevance feedback, by viewing it as a three component mixture model of document, set of feedback documents, and collection. Our approach is more straightforward, since it considers each feedback document separately and, hence, does not require the additional mixture model parameter. To create parsimonious language models we use an EM algorithm to update the maximum-likelihood (ML) estimates. Zhai and Lafferty already proposed an approach which uses a similar EM algorithm; it differs, however, in the way the set of feedback documents is handled. Whereas we parsimonize each individual document, they apply their EM algorithm to the entire set of feedback documents.

To verify our hypothesis, we use a specific instance of blind relevance feedback, namely relevance modeling (RM). We choose this particular method because it has been shown to achieve state-of-the-art retrieval performance. Relevance modeling assumes that the query and the set of documents are samples from an underlying term distribution—the relevance model. Lavrenko and Croft formulate two ways of approaching the estimation of the parameters of this model. We build upon their work and compare the results of our proposed parsimonious relevance models with RMs as well as with a query-likelihood baseline. To measure the effects in different contexts, we employ five test collections taken from the TREC-7, TREC Robust, Genomics, Blog, and Enterprise tracks and show that our proposed model improves performance in terms of mean average precision on all the topic sets over both a query-likelihood baseline as well as a run based on relevance models. Moreover, although blind relevance feedback is mainly a recall enhancing technique, we observe that parsimonious relevance models (unlike their non-parsimonized counterparts) can also improve early precision and reciprocal rank of the first relevant result. Thus, our parsimonious relevance models (i) improve retrieval effectiveness in terms of MAP on all collections, (ii) significantly outperform their non-parsimonious counterparts on most measures, and (iii) have a precision enhancing effect, unlike other blind relevance feedback methods.

\[bibtex key=SIGIR:2008:Meij-prm\]

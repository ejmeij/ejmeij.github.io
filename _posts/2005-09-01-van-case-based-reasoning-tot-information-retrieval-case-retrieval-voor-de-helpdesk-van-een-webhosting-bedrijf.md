---
layout: default
title: "Van Case-Based Reasoning tot Information Retrieval; Case retrieval voor de helpdesk van een webhosting bedrijf"
date: "2005-09-01"
categories:
  - "publication"
  - "theses"
tags:
  - "a-research-thesis-in-case-based-reasoning-applied-to-information-retrieval"
  - "case-based-reasoning"
  - "case-based-reasoning-papers-2011"
  - "case-based-retrieval-methods"
  - "case-retrieval-methods-in-case-based-reasoning"
  - "edgar-meij-hostnet"
  - "faq"
  - "information-retrieval"
  - "information-based-resionnig"
  - "information-retrieval-helpdesk"
  - "mean-reciprocal-rank"
  - "mean-reciprocal-rank-case-based-retrieval"
  - "mean-reciprocal-rank-research-paper"
  - "mrr-mean-reciprocal-rank"
  - "phd-thesis-on-case-based-reasoning-for-post-retrieval"
  - "reciprocal-rank"
  - "research-papers-on-mean-reciprocal-rank"
  - "resoning-based-of-ranks"
  - "retrieval-techniques-in-case-based-reasoning"
  - "thesis-case-based-reasoning-semantic"
coverImage: "hostnet.png"
---

The helpdesk department of Hostnet, a web hosting company, daily receives 35 up to 50 questions from its customers. Within the domain in which Hostnet operates, only few off-the-shelf manuals exist and this is particularly noticeable on the helpdesk. Currently, only a few possibilities for knowledge management and/or elicitation exist within the organization. Questions are answered and problems are solved mostly by relying on the expertise of the staff. They therefore need to have up-to-date knowledge of a variety of possible questions, problem situations and solutions. They also need to be creative and flexible when handling novel questions.

Hostnet uses a ticketing system to handle questions from their customers. One of many advantages of using such a system is that all questions are stored, along with their corresponding answers. Hostnet uses the system for some time now and it has thus collected a large amount of domain and organization specific knowledge. This kind of information is exactly the type on which the research area of case-based reasoning focuses. Case-based reasoning uses previously solved problems (cases) as a knowledge source to aid solving similar cases in the future. One of the main components, in any case-based reasoning system, is the retrieval module. This module searches for alike cases, given a new case and a similarity measure. Techniques from the area of Information Retrieval may be used to assist in finding these alike questions, for example by implementing vector-space based, statistical methods. This research focuses on analyzing to what extent previously solved cases can serve as a basis for a statistical information retrieval module of a case-based reasoning system within Hostnet by measuring the effects of different information retrieval techniques on the results. The evaluated techniques are stemming, term weighting and combinations thereof. The above described organizational setting is not unique to Hostnet. Every service-providing company with direct customer contacts is probably familiar with the described situation and could benefit from the presented results.

The suggested approach yields adequate results by which, at best, 60% of new questions can be answered, based on the first 10 retrieved stored questions. The mean reciprocal rank of the first matching question provided room for improvement however, with a value of 7 out of 10. The most important conclusion is that the best results are achieved when applying none of the before mentioned information retrieval techniques. The suggested approach needs to be improved for a successful integration within a case-based reasoning system, but it does seem viable.

\[bibtex key=2005:meij\]

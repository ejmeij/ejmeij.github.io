---
title: "DutchHatTrick: Semantic query modeling, ConText, section detection, and match score maximization."
date: "2012-01-25"
categories: 
  - "publication"
  - "unrefereed"
tags: 
  - "dutchhattrick"
  - "entity-linking"
  - "nlp-repository-at-pittsburgh"
  - "pittsburgh-university-trec-med"
  - "query-modeling"
  - "repository-semantic-slang"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semantic-slang"
  - "trec-medical"
  - "trec-2011-data"
  - "trec-2011-twitter-data"
  - "trec-2011tweets-2011"
  - "trec-medical-topics"
  - "trec-twitter-2011-data-format"
  - "trec2011workingnotestrecmedicalrecords"
  - "tweet-format-trec"
  - "twitter-trec"
  - "university-medical-nlp"
  - "university-of-pittsburgh-nlp-repository-medical-reports-format"
  - "what-is-a-medical-trec"
coverImage: "paper_3.png"
---

This report discusses the collaborative work of the ErasmusMC, University of Twente, and the University of Amsterdam on the TREC 2011 Medical track. Here, the task is to retrieve patient visits from the University of Pittsburgh NLP Repository for 35 topics. The repository consists of 101,711 patient reports, and a patient visit was recorded in one or more reports.

Because the training set provided by the track organization was small and not made available until quite late in the competition, we decided to create a small training set ourselves. Not only did this allow us to test several ideas before submitting runs to TREC, it also led to several insights into the data. One finding was that synonyms are widely used. Query expansion was therefore deemed essential to achieve a reasonable performance. Query expansion has been used before in Information Retrieval (IR), and is often divided into statistical and knowledge-based query expansion. Statistical query expansion uses data derived from the corpus itself, and a well-known example is pseudo-relevance feedback . In contrast, we investigated knowledge-based query expansion, which uses a knowledge base such as an ontology or a dictionary to find related terms. This type of query expansion has not always proven to be successful. For instance, Hersh et al. found a decrease in overall search performance when using the Unified Medical Language System (UMLS) to find related terms. Liu et al. found slight improvements with scenario-specific expansion strategies using UMLS. In a previous TREC track, we also found reduced performance when using concept based query expansion , but found slightly improved results when using an approach combining concepts with a statistical model of related words . Similarly, Zhou found promising results when using combination of both the original words in the text and the synonyms found for concepts in the text.

An often-used resource for knowledge-based query expansion in the biomedical domain is the UMLS. However, initial explorations indicated that there is only limited overlap between terms used in topics and medical records and terms found in the UMLS. The main reason for this appears to be that the UMLS is mainly constructed from vocabularies used in classifying clinical data, but not intended to be used in text- mining. Terms in the UMLS tend to be more specific than what a physician would use in free-text reporting. For instance, a physician might use the term „upper endoscopy‟, but this term is not found in the UMLS. Instead, the term „upper GI endoscopy‟ is found. We have therefore explored a different source of synonyms: Wikipedia. We expected Wikipedia to have a better coverage of the terms encountered in medical records.

\[bibtex key=TREC:2011:schuemie\]

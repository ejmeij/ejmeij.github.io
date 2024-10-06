---
title: "Structuring and extracting knowledge for the support of hypothesis generation in molecular biology"
date: "2009-10-20"
categories:
  - "conference"
  - "publication"
tags:
  - "aida"
  - "api-untuk-text-mining"
  - "api-untuk-web"
  - "mining-from-twitter"
  - "text-mining"
  - "text-mining-twitter"
  - "text-mining-twitter-api"
  - "text-mining-with-twitter-article"
  - "twitter-api-for-text-mining"
  - "twitter-text-mining"
  - "web-services"
  - "web-service-untuk-text-mining"
  - "workflows"
coverImage: "bmc.png"
---

Hypothesis generation in molecular and cellular biology is an empirical process in which knowledge derived from prior experiments is distilled into a comprehensible model. The requirement of automated support is exemplified by the difficulty of considering all relevant facts that are contained in the millions of documents available from PubMed. Semantic Web provides tools for sharing prior knowledge, while information retrieval and information extraction techniques enable its extraction from literature. Their combination makes prior knowledge available for computational analysis and inference. While some tools provide complete solutions that limit the control over the modeling and extraction processes, we seek a methodology that supports control by the experimenter over these critical processes.

We describe progress towards automated support for the generation of biomolecular hypotheses. Semantic Web technologies are used to structure and store knowledge, while a workflow extracts knowledge from text. We designed minimal proto-ontologies in OWL for capturing different aspects of a text mining experiment: the biological hypothesis, text and documents, text mining, and workflow provenance. The models fit a methodology that allows focus on the requirements of a single experiment while supporting reuse and posterior analysis of extracted knowledge from multiple experiments. Our workflow is composed of services from the 'Adaptive Information Disclosure Application' (AIDA) toolkit as well as a few others. The output is a semantic model with putative biological relations, with each relation linked to the corresponding evidence.

We demonstrated a 'do-it-yourself' approach for structuring and extracting knowledge in the context of experimental research on biomolecular mechanisms. The methodology can be used to bootstrap the construction of semantically rich biological models using the results of knowledge extraction processes. Models specific to particular experiments can be constructed that, in turn, link with other semantic models, creating a web of knowledge that spans experiments. Mapping mechanisms can link to other knowledge resources such as OBO ontologies or SKOS vocabularies. AIDA Web Services can be used to design personalized knowledge extraction procedures. In our example experiment, we found three proteins (NF-Kappa B, p21, and Bax) potentially playing a role in the interplay between nutrients and epigenetic gene regulation.

\[bibtex key=BMC:2009:roos\]

---
title: "Biological applications of Aida knowledge management components"
date: "2008-03-16"
categories:
  - "conference"
  - "publication"
tags:
  - "aida"
  - "aida-knowledge"
  - "applications-of-aida"
  - "marco-roos-aida"
  - "web-services"
  - "workflows"
coverImage: "process.jpg"
---

Given the important role of knowledge in biology, knowledge in a machine readable form can be an important asset for bioinformatics. We present two applications of AIDA (Adaptive Information Disclosure Application), a collection of knowledge management components. One is a workflow that extends a semantic model with putative relations between proteins and diseases extracted from literature by machine learning techniques. The other extends vBrowser, a virtual resource browser tool, with the ability to find relevant biological resources (e.g. data, workflows, documents) via semantic relationships.

Central to our semantic web approach is the separation of a ‘virtual knowledge space’ from its applications. In other words, knowledge is disclosed and accessed in a knowledge space rather than being coded into the application. The workflow adds knowledge to this space with knowledge extraction, while vBrowser accesses the knowledge resources for use during search. We use RDF and OWL to represent knowledge and Sesame to store RDF and OWL representations of knowledge.

The workflow contains the following steps: (i) add the ontology that you want to extend to Sesame (e.g. a model that contains the protein EZH2), (ii) extract the entities of interest from the ontology (e.g. EZH2), (iii) retrieve abstracts from Medline for these entities, (iv) extract proteins and protein-protein relationships from the abstracts, (v) add a ranking score to the discoveries, (vi) query OMIM with the extracted proteins and retrieve the disease labels (service from the National Institute of Genetics in Japan), (vii) add the discoveries and their interrelationships to the repository, (viii) export the enriched ontology to the knowledge space where for instance vBrowser can be used to explore the results. Future work includes metrics to more effectively retrieve biologically interesting suggestions from semantic data.

We show how the vBrowser can be used to browse both data resources and knowledge resources from the same basic interface. We show how vBrowser uses an AIDA thesaurus service to improve finding resources such as Medline documents and workflows on myExperiment.org. We found thesauri terms effective for search and advocate SKOS for its intuitive ‘broader/narrower-than’ relationships. We further show that the protein-disease relationships resulting from our knowledge capture workflow as well as the documents that contained these relationships can be accessed as knowledge resources from the vBrowser. We think OWL can adequately represent the knowledge in many biological cartoon models and have used it to represent the workflow provenance in our knowledge capture workflow.

\[bibtex key=ISMB:2008:roos\]

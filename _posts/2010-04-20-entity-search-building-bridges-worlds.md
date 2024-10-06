---
title: "Entity Search: Building Bridges between Two Worlds"
date: "2010-04-20"
categories:
  - "publication"
  - "workshop"
tags:
  - "edgar-entity-search"
  - "edgar-meij-yahoo"
  - "edgar-sparql"
  - "edger-entity-search"
  - "entity-linking"
  - "entity-oriented-search-semantic-search"
  - "entity-retrieval-in-web-searchingpdf"
  - "entity-search-and-lod-research-issues"
  - "information-retrieval"
  - "is-known-as-entity"
  - "linking-open-data"
  - "lod"
  - "meij-entities"
  - "semantic-linking"
  - "semantic-query-analysis"
  - "semantic-search"
  - "trec-entity"
  - "trec-2013-entity-search"
  - "trec-entity-track-2011-queries"
  - "trec-retrieval"
coverImage: "semsearch2010.png"
---

We have come to depend on technological resources to create order and find meaning in the ever-growing amount of online data. One frequently recurring type of query in web search are queries containing named entities (persons, organizations, locations, etc.): we organize our environments around entities that are meaningful to us. Hence, to support humans in dealing with massive volumes of data, next generation search engines need to organize information in semantically meaningful ways, structured around entities. Furthermore, instead of merely finding documents that mention an entity, finding the entity itself is required.

The problem of entity search has been and is being looked at by both the Information Retrieval (IR) and Semantic Web (SW) communities and is, in fact, ranked high on the research agendas of the two communities. The entity search task comes in several flavors. One is known as entity ranking (given a query and target category, return a ranked list of relevant entities), another is list completion (given a query and example entities, return similar entities), and a third is related entity finding (given a source entity, a relation and a target type, identify target entities that enjoy the specified relation with the source entity and that satisfy the target type constraint).

State-of-the-art IR models allow us to address entity search by identifying relevant entities in large volumes of web data. These methods often approach entity-oriented retrieval tasks by establishing associations between topics, documents, and entities or amongst entities themselves, where such associations are modeled by observing the language usage around entities. A major challenge with current IR approaches to entity retrieval is that they fail to produce interpretable descriptions of the found entities or of the relationships between entities. The generated models tend to lack human-interpretable semantics and are rarely meaningful for human consumption: interpretable labels are needed (both for entities and for relations). Linked Open Data (LOD) is a recent contribution of the emerging semantic web that has the potential of providing the required semantic information.

From a SW point of view, entity retrieval should be as simple as running SPARQL queries over structured data. However, since a true semantic web still has not been fully realized, the results of such queries are currently not sufficient to answer common information needs. By now, the LOD cloud contains millions of concepts from over one hundred structured data sets. This abundance, however, also introduces novel issues such as “cheap semantics” (e.g. wikilink relations in DBpedia) and the need for ranking potentially very large amounts of results. Furthermore, given the fact that most web users are not proficient users of semantic web languages such as SPARQL or standards such as RDF and OWL, the free-form text input used by most IR systems is more appealing to end users.

These concurrent developments give rise to the following general question: to which extent are state-of-art IR and SW technologies capable of answering information needs related to entity finding? In this paper we focus on the task of related entity finding (REF). E.g., for a source entity (“Michael Schumacher”), a relation (“Michael’s teammates while he was racing in Formula 1”) and a target type (“people”), a REF system should return entities such as “Eddie Irvine” and “Felipe Massa.” REF aims at making arbitrary relations between entities searchable. We focus on an adaptation of the official task as it was run at TREC 2009 and restrict the target entities to those having a primary Wikipedia article: this modification provides an elegant way of making the IR and SW results comparable.

From an IR perspective, a natural way of capturing the relation between a source and target entity is based on their co-occurrence in suitable contexts. Later, we use an aggregate of methods all of which are based on this approach. In contrast, a SW perspective on the same task is to search for entities through links such as the ones in LOD and for this we apply both standard SPARQL queries and an exhaustive graph search algorithm.

In this paper, we analyze and discuss to which extent REF can be solved by IR and SW methods. It is important to note that our goal is not to perform a quantitative comparison, and make claims about one approach being better than the other or vice versa. Rather, we investigate results returned by either approach and perform a more qualitative evaluation. We find that IR and SW methods discover different sets of entities, although these sets are overlapping. Based on the results of our evaluation, we demonstrate that the two approaches are complementary in nature and we discuss how each field could potentially benefit from the other. We arrive at and motivate a proposal to combine text-based entity models with semantic information from the Linking Open Data cloud.

\[bibtex key=semsearch:2010:balog\]

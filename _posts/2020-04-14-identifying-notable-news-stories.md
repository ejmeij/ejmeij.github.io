---
title: "Identifying Notable News Stories"
date: "2020-04-14"
categories: 
  - "blog"
  - "conference"
  - "publication"
tags: 
  - "information-retrieval"
  - "knowledge-graph"
coverImage: "ECIR2020-e1614421462762.jpeg"
---

The volume of news content has increased significantly in recent years and systems to process and deliver this information in an automated fashion at scale are becoming increasingly prevalent. One critical component that is required in such systems is a method to automatically determine how notable a certain news story is, in order to prioritize these stories during delivery. One way to do so is to compare each story in a stream of news stories to a notable event. In other words, the problem of detecting notable news can be defined as a ranking task; given a trusted source of notable events and a stream of candidate news stories, we aim to answer the question: “Which of the candidate news stories is most similar to the notable one?”. We employ different combinations of features and learning to rank (LTR) models and gather relevance labels using crowdsourcing. In our approach, we use structured representations of candidate news stories (triples) and we link them to corresponding entities. Our evaluation shows that the features in our proposed method outperform standard ranking methods, and that the trained model generalizes well to unseen news stories.

\[bibtex key=ECIR:2020:Saravanou\]

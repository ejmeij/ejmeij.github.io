---
layout: default
title: "Evaluating the Calibration of Knowledge Graph Embeddings for Trustworthy Link Prediction"
date: "2020-11-16"
categories:
  - "blog"
  - "conference"
  - "publication"
tags:
  - "httpsedgar-meij-pro"
coverImage: "adNEfAT4-e1614421393177.jpg"
---

Little is known about the trustworthiness of predictions made by knowledge graph embedding (KGE) models. In this paper we take initial steps toward this direction by investigating the calibration of KGE models, or the extent to which they output confidence scores that reflect the expected correctness of predicted knowledge graph triples. We first conduct an evaluation under the standard closed-world assumption (CWA), in which predicted triples not already in the knowledge graph are considered false, and show that existing calibration techniques are effective for KGE under this common but narrow assumption. Next, we introduce the more realistic but challenging open-world assumption (OWA), in which unobserved predictions are not considered true or false until ground-truth labels are obtained. Here, we show that existing calibration techniques are much less effective under the OWA than the CWA, and provide explanations for this discrepancy. Finally, to motivate the utility of calibration for KGE from a practitioner’s perspective, we conduct a unique case study of human-AI collaboration, showing that calibrated predictions can improve human performance in a knowledge graph completion task.

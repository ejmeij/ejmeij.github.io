---
layout: default
title: "Similarity-based Multi-Domain Dialogue State Tracking with Copy Mechanisms for Task-based Virtual Personal Assistants (WWW 2022)"
date: "2022-04-09"
categories:
  - "blog"
  - "conference"
  - "publication"
---

Task-based Virtual Personal Assistants (VPAs) rely on multi-domain Dialogue State Tracking (DST) models to monitor goals throughout a conversation. Previously proposed models show promising results on established benchmarks, but they have difficulty adapting to unseen domains due to domain-specific parameters in their model architectures. We propose a new Similarity-based Multi-domain Dialogue State Tracking model (SM-DST) that uses retrieval-inspired and fine-grained contextual token-level similarity approaches to efficiently and effectively track dialogue state. The key difference with state-of-the-art DST models is that SM-DST has a single model with shared parameters across domains and slots. Because we base SM-DST on similarity it allows the transfer of tracking information between semantically related domains as well as to unseen domains without retraining. Furthermore, we leverage copy mechanisms that consider the system’s response and the dialogue state from previous turn predictions, allowing it to more effectively track dialogue state for complex conversations. We evaluate SM-DST on three variants of the MultiWOZ DST benchmark datasets. The results demonstrate that SM-DST significantly and consistently outperforms state-of-the-art models across all datasets by absolute 5-18% and 3-25% in the few- and zero-shot settings, respectively.

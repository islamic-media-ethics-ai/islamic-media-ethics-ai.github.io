---
layout: post
title: Paper accepted at ACL 2026
date: 2026-04-07 15:59:00-0400
inline: false
related_posts: true
---

We are happy to share that our paper **"From RAG to Agentic RAG for Faithful Islamic
Question Answering"** has been accepted at **ACL 2026**.

---

## Overview

Large Language Models (LLMs) are increasingly being used to answer questions on Islamic topics.
However, ungrounded or hallucinated responses in this domain carry serious religious and
ethical consequences. Standard multiple-choice or reading-comprehension benchmarks fail to
capture these real-world failure modes — in particular, free-form hallucinations and the
failure to appropriately abstain when supporting evidence is absent.

This paper addresses these gaps head-on, introducing a comprehensive suite of resources and
an agentic framework designed to make Islamic QA systems more faithful, grounded, and
trustworthy.

---

## Key Contributions

### 🗂️ ISLAMICFAITHQA Benchmark
We introduce **ISLAMICFAITHQA**, a new bilingual (Arabic/English) generative benchmark
comprising **3,810 items** with atomic single-gold answers. Unlike prior MCQ-style datasets,
this benchmark is specifically designed to enable direct measurement of hallucination rates
and appropriate abstention behavior — both critical dimensions for responsible Islamic QA.

### 🛠️ End-to-End Grounded Modelling Suite
To support model training and alignment, we developed a rich resource package:
- **25,000** Arabic text-grounded supervised fine-tuning (SFT) reasoning pairs
- **5,000** bilingual preference samples for reward-guided alignment
- A verse-level **Qur'an retrieval corpus** of **6,236 atomic ayat (verses)**

### 🤖 Agentic RAG Framework
Building on these resources, we propose an **Agentic Quran-grounding framework** that moves
beyond standard Retrieval-Augmented Generation (RAG). The system employs structured tool
calls for *iterative evidence seeking and answer revision*, enabling models to dynamically
search for and validate Qur'anic support before committing to a response. This yields more
faithful, citation-backed answers compared to vanilla RAG pipelines.

---

## Why It Matters

Islamic question answering sits at the intersection of AI, language, and religious
scholarship. A model that confabulates an Islamic ruling — even confidently — can mislead
users on matters of deep personal and communal significance. By combining rigorous
benchmarking, large-scale grounded training data, and an agentic evidence-seeking pipeline,
this work takes a meaningful step toward AI systems that know *when* to answer and *when*
to defer — a capability as important as accuracy itself.

---

## Authors

Gagan Bhatia, Hamdy Mubarak, Mustafa Jarrar, George Mikros, Fadi Zaraket, Mahmoud
Alhirthani, Mutaz Al-Khatib, Logan Cochrane, Kareem Darwish, Rashid Yahiaoui, and
**Firoj Alam**

*Qatar Computing Research Institute (QCRI), HBKU · College of Humanities and Social
Sciences, HBKU · Arab Center for Research and Policy Studies · College of Islamic
Studies, HBKU*

---

## 📄 Read the Paper

The full paper is available on arXiv:
**[https://arxiv.org/abs/2601.07528](https://arxiv.org/abs/2601.07528)**

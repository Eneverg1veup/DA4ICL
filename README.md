# DA4ICL
**Beyond Plain Demos: A Demo-centric Anchoring Paradigm for In-Context Learning in Alzheimer’s Disease Detection (AAAI 2026)**

![Status](https://img.shields.io/badge/Status-Preparing%20Release-yellow)
![Conference](https://img.shields.io/badge/AAAI-2026-blue)
![Topic](https://img.shields.io/badge/NLP-ICL%20%7C%20Task%20Vectors%20%7C%20AD%20Detection-6f42c1)

> **NEWS — 2025/11/08**: Our paper is **accepted by AAAI 2026** (🎉).  
> **TODO**: Code, configs, and datasets will be released after organization.

---

## TL;DR
**DA4ICL** improves ICL for Alzheimer’s disease (AD) detection by (1) **Diverse & Contrastive Retrieval (DCR)** to widen the demo context and (2) **Projected Vector Anchoring (PVA)** to deepen demo signals at every Transformer layer. It yields stable gains over both standard ICL and task-vector (TV) baselines on multiple AD benchmarks.

---

## Abstract
Detecting Alzheimer’s disease (AD) from narrative transcripts challenges large language models (LLMs): pre-training rarely covers this out-of-distribution task, and all transcript demos describe the same scene, producing highly homogeneous contexts. These factors cripple both the model’s built-in task knowledge (**task cognition**) and its ability to surface subtle, class-discriminative cues (**contextual perception**). Because cognition is fixed after pre-training, improving in-context learning (ICL) for AD detection hinges on enriching perception through better demonstration (demo) sets. We show that standard ICL quickly saturates—its demos lack diversity (**context width**) and fail to convey fine-grained signals (**context depth**). Although recent task-vector (TV) methods adapt models by injecting TVs into hidden states, they are ill-suited for AD detection due to mismatches in **injection granularity, strength, and position**.  
To address these bottlenecks, we introduce **DA4ICL**, a demo-centric anchoring framework that **widens** context via **Diverse & Contrastive Retrieval (DCR)** and **deepens** each demo’s signal via **Projected Vector Anchoring (PVA)** across Transformer layers. Across three AD benchmarks, DA4ICL achieves large, stable gains over ICL and TV baselines, charting a new paradigm for fine-grained, OOD, and low-resource LLM adaptation.

---

## Method Overview
- **DCR — Diverse & Contrastive Retrieval**  
  Curates a main-demo set with **complementary roles** (similar vs. contrastive) to expand context width under strong semantic homogeneity.
- **PVA — Projected Vector Anchoring**  
  Performs **layer-wise** projection and controlled anchoring to inject fine-grained, class-discriminative signals without misalignment or over-injection.

---

## Repository Structure (planned)

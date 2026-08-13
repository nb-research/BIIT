# BIIT — Benchmark for Indic Industrial TTS

**BIIT** is a deployment-oriented benchmark for evaluating text-to-speech (TTS) systems on Indian production workloads. It pairs a structured, deployment-focused text corpus with an evaluation suite that scores TTS systems on perceptual quality, intelligibility, acoustic and prosodic fidelity, speaker similarity, and latency/throughput across T4, L4, and A100 GPUs.

This repository accompanies the paper:

> **Adapting Indic Text-to-Speech for the Real World: A Survey of Architectures and an Industrial-Grade Benchmark**
> Boneshwar V. K., Udeshya Raj, Ishan Grover, and Zaher Abdul Azeez
> *Preprint.*

## Overview

Generative TTS has advanced faster than the field's ability to compare systems on what production actually demands: intelligibility on dense numerals and code-mixed input, faithful speaker identity, and latency under realistic serving budgets — especially for low-resource Indic languages and Indian industrial use cases. BIIT is built to close that gap.

The accompanying work contributes:

- An **architecture-driven taxonomy** organizing recent TTS systems into six families (autoencoder/GAN, autoregressive, diffusion and flow-matching, codec-based, modern hybrid, and full-duplex speech-to-speech), annotated with parameter scale and practitioner-facing axes.
- The **BIIT corpus**, a deployment-oriented text benchmark grounded in Indian enterprise workflows.
- A **benchmark of highly-ranked open-source TTS systems** under a single frozen reference, spanning quality, intelligibility, prosodic fidelity, speaker similarity, and deployment metrics across three GPU classes.

## Dataset

BIIT is a **text-only** corpus, curated so that synthesis is decoupled from dataset design and every system is compared on the same items.

- **10,672 utterances** organized under a fixed taxonomy of **46 base categories**.
- **10 Indic languages** (Hindi, Tamil, Bengali, Telugu, Marathi, Gujarati, Kannada, Malayalam, Assamese, Punjabi) plus an **English baseline**, across **9 scripts**, each Indic language in its native script.
- Grounded in **24 industry sectors**, with emphasis on banking, financial services, and insurance (BFSI) and customer-facing voice automation.
- Coverage spans linguistic stress cases (phone numbers, lakh–crore numerals, currency and EMI expressions, date variants, regulatory abbreviations, complex Indian names, and authentic code-mixing), scenario-grounded enterprise conversations, prosody-focused sets, paraphrase pairs, and long-form / multi-turn prompts.
- Per-item annotations (reference text, category metadata, expected-prosody descriptors, pre-localized and severity-typed error spans, and item-level criticality grades) drive the metric suite directly, enabling severity-weighted evaluation that weights deployment-blocking failures above minor prosodic slips.

## Availability

**The BIIT benchmark dataset is available on demand.** It is released strictly for research and evaluation purposes. To request access, please email **udeshayraj@gmail.com** with a brief description of your intended use. Sensitive scenario content carries usage restrictions and is governed accordingly.

## Citation

If you use BIIT, please cite the paper. A full citation (BibTeX) will be added here upon publication.

## Contact

For dataset access requests and questions, please email **udeshayraj@gmail.com**.


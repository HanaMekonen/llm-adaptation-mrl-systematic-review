# Standardized Data Extraction Template

**Appendix D: Data Extraction Template**

This repository contains the standardized data extraction template used in the systematic review:

> **Techniques for Adapting Large Language Models to Low-Resource, Morphologically Rich Languages: A Systematic Review**

The template was developed before full-text review to ensure consistent and reproducible extraction of evidence across all included studies.

---

# General Instructions

Complete **one extraction form for each included primary study**.

Extraction should always be performed from the **full text** rather than the abstract.

If information is unavailable, use the following standardized codes.

| Code | Meaning |
|-------|---------|
| **NR** | Not Reported |
| **NA** | Not Applicable |
| **EST** | Estimated from reported information |

---

## File Naming Convention

Save each extraction using

```
PXX_FirstAuthor_Year.md
```

Example

```
P22_Vemula_2025.md
```

---

# Data Extraction Form

---

# 1. Study Metadata

| Field | Value |
|-------|-------|
| Paper ID | |
| Authors | |
| Year | |
| Publication Type | Journal / Conference / Workshop |
| Venue | |
| DOI | |
| Country of First Author (optional) | |

---

# 2. Language and Typological Characteristics

Record **every language evaluated in the study**.

For multilingual studies, list all languages and indicate the role of each.

| Field | Value |
|-------|-------|
| Target Language(s) | |
| Source Language(s) | |
| Evaluation Language(s) | |
| Language Family | |
| Writing System / Script | |
| Morphological Typology | |
| Typology Source | WALS / Glottolog / Ethnologue / Linguistic literature / Study definition / Other |
| Resource Level | High / Medium / Low |
| Resource Level Definition | Definition used by the authors (if reported) |
| Language Role | Source / Target / Evaluation / Multiple |

---

# 3. Foundation Model Characteristics

| Field | Value |
|-------|-------|
| Base Model | |
| Model Size | |
| Architecture | Decoder-only / Encoder-only / Encoder-Decoder |
| Model Availability | Open-weight / Proprietary |
| Original Training Objective | Causal LM / MLM / Seq2Seq / Other |

---

# 4. Adaptation Strategy

| Field | Value |
|-------|-------|
| Primary Adaptation Technique | |
| Continued Pretraining | |
| PEFT Method | LoRA / QLoRA / IA³ / ReFT / Adapter / Other |
| Prompting Strategy | Zero-shot / Few-shot / CoT / Self-refine / Other |
| Tokenizer Adaptation | |
| Vocabulary Expansion | |
| Retrieval-Augmented Generation (RAG) | |
| Cross-lingual Transfer | |
| Hybrid Pipeline | |
| Important Hyperparameters | Rank, α, learning rate, epochs, etc. |

---

# 5. Training Configuration

| Field | Value |
|-------|-------|
| Training Corpus | |
| Corpus Size | |
| Data Source | |
| GPU Hardware | |
| GPU Memory | |
| Training Time | |
| Total Parameters | |
| Trainable Parameters | |
| Energy or Cost Reported | Yes / No |

---

# 6. Evaluation

| Field | Value |
|-------|-------|
| Downstream Task(s) | |
| Evaluation Type | Generative / Discriminative |
| Benchmark Dataset(s) | |
| Evaluation Metrics | |
| Baselines | |
| Number of Experimental Runs | |
| Variance Reported | Yes / No |
| Statistical Tests | |
| Error Analysis | Yes / No |

---

# 7. Main Results

| Field | Value |
|-------|-------|
| Main Findings | |
| Key Quantitative Results | |
| Computational Efficiency | |
| Reported Limitations | |

---

# 8. Contribution to Research Questions

| RQ | Contribution | Evidence |
|----|-------------|----------|
| RQ1 | Adaptation techniques | |
| RQ2 | Quantitative comparison | |
| RQ3 | Influence of morphology and typology | |
| RQ4 | Evaluation practices | |

---

# 9. Quality Assessment

Each study is evaluated using three predefined criteria.

## Criterion 1 — Reporting Clarity

| Rating | Description |
|---------|-------------|
| High | Architecture, datasets, hyperparameters, and methodology fully described |
| Medium | Minor methodological details missing |
| Low | Important methodological information missing |

---

## Criterion 2 — Baseline Appropriateness

| Rating | Description |
|---------|-------------|
| High | Compared with strong and appropriate baselines |
| Medium | Compared with limited baselines |
| Low | Weak or missing baseline comparison |

---

## Criterion 3 — Evaluation Robustness

| Rating | Description |
|---------|-------------|
| High | Multiple datasets/tasks, repeated runs, variance or significance testing reported |
| Medium | Adequate evaluation but limited robustness reporting |
| Low | Minimal evaluation or insufficient experimental evidence |

---

### Overall Assessment

| Criterion | Rating | Justification |
|-----------|--------|---------------|
| Reporting Clarity | | |
| Baseline Appropriateness | | |
| Evaluation Robustness | | |
| Overall Quality | High / Medium / Low | |

---

# 10. Reproducibility

| Field | Value |
|-------|-------|
| Code Available | |
| Model Available | |
| Dataset Available | |
| Experimental Details Sufficient | |
| License | |

---

# 11. Reviewer Notes

| Field | Notes |
|-------|------|
| Methodological Concerns | |
| Interesting Technical Details | |
| Relevance to Narrative Synthesis | |
| Additional Observations | |

---

# Example Completed Extraction

The repository includes one fully completed example:

```
P22_Vemula_2025.md
```

This example illustrates the expected level of detail and formatting for all extracted studies.

### 1. Study Metadata

| Field | Value |
| :--- | :--- |
| **Paper ID** | P22 |
| **Authors** | Saketh Reddy Vemula, Sandipan Dandapat, Dipti Misra Sharma, Parameswari Krishnamurthy |
| **Year** | 2025 |
| **Publication Type** | Conference paper |
| **Venue** | IJCNLP-AACL 2025 |
| **DOI** | 10.18653/v1/2025.ijcnlp-srw.20 |

---

### 2. Language and Typological Characteristics

| Field | Value |
| :--- | :--- |
| **Target Language(s)** | Telugu, Hindi, English |
| **Language Family** | Dravidian (Telugu); Indo-Aryan (Hindi); Indo-European (English) |
| **Writing System / Script** | Telugu, Devanagari, Latin |
| **Morphological Typology** | Agglutinative (Telugu); Fusional with agglutination (Hindi); Fusional (English) |
| **Typology Source** | Established linguistic literature |
| **Resource Level** | Low-resource (Telugu, Hindi); High-resource (English) |
| **Resource Level Definition** | Not reported |
| **Language Role** | Target and Evaluation |

---

### 3. Model Characteristics

| Field | Value |
| :--- | :--- |
| **Base Model** | BERT (custom trained from scratch) |
| **Model Size** | 8.5M (excluding embedding layer) |
| **Model Availability** | Open-weight |
| **Architecture** | Encoder-only |

---

### 4. Adaptation Strategy

| Field | Value |
| :--- | :--- |
| **Training Objective** | Masked Language Modeling |
| **Continued Pretraining** | No |
| **Parameter-Efficient Fine-Tuning (PEFT)** | None (full training from scratch) |
| **Prompting** | None |
| **Tokenizer Adaptation** | Unigram, BPE, Morfessor+BPE, Morphological Analyzer+BPE, Word-level |
| **Vocabulary Expansion** | Yes — 8K, 16K, 50K vocabulary sizes |
| **Retrieval-Augmented Generation (RAG)** | Not applicable |
| **Hybrid Adaptation Pipeline** | Not applicable |

---

### 5. Training Configuration

| Field | Value |
| :--- | :--- |
| **Training Corpus** | WMT News Crawl + IndicCorp (Telugu) |
| **Training Data Size** | 10M sentences per language |
| **Data Source** | WMT News Crawl, IndicCorp |
| **GPU** | NVIDIA RTX 6000 (pre-training), 4× RTX 2080 (fine-tuning) |
| **GPU Memory** | 50GB VRAM (pre-training) |
| **Model Parameters** | 8.5M (excluding embedding layer) |
| **Trainable Parameters** | 8.5M (full training) |
| **Training Time** | 175,000 steps |

---

### 6. Evaluation

| Field | Value |
| :--- | :--- |
| **Task** | Text Classification, POS Tagging, NER, Dependency Parsing, Similarity Assessment, NLI |
| **Evaluation Type** | Discriminative |
| **Evaluation Dataset** | IndicGLUE, IndicXTREME, GLUE |
| **Evaluation Metrics** | Accuracy, F1, LAS, Pearson/Spearman correlation |
| **Baseline Models** | BPE, Character-level, Word-level, Morfessor, Morphological Analyzer |
| **Experimental Runs** | 3 independent runs |
| **Statistical Analysis** | ANOVA, ANCOVA, fixed-effects models with p-values |

---

### 7. Results

| Field | Value |
| :--- | :--- |
| **Main Findings** | Unigram outperforms BPE on agglutinative Telugu (MorphScore F1=0.79 vs 0.27); morphological alignment shows moderate positive correlation with syntax-based tasks; hybrid approaches boost BPE but not Unigram |
| **Limitations** | Encoder-only models only; small model size (8.5M); limited to NLU tasks |
| **Key Quantitative Results** | MorphScore F1: Unigram=0.79, BPE=0.27; Word similarity: Unigram=89.4%, BPE=79.7%; Unigram > BPE for Telugu across most settings |
| **Computational Cost** | 72 models pre-trained; 2,160+ fine-tuning runs |

---

### 8. Evidence for Research Questions

| RQ | Contribution | Yes/No | Evidence Description |
| :--- | :--- | :--- | :--- |
| **RQ1** | Adaptation techniques and mechanisms | ☑ Yes | Tokenization (Unigram vs. BPE), morphological alignment, hybrid tokenizers |
| **RQ2** | Quantitative comparison (data, compute, performance) | ☑ Yes | Detailed comparison across vocabulary sizes, tokenizer variants, and tasks |
| **RQ3** | Typology influence on adaptation | ☑ Yes | Agglutinative Telugu: Unigram > BPE; morphological alignment correlates with syntax tasks |
| **RQ4** | Evaluation, benchmarks, and metrics | ☐ No | Not addressed |

---

### 9. Quality Assessment

| Criterion | Rating | Justification |
| :--- | :--- | :--- |
| **Reporting Clarity (C1)** | ☑ H | Full architectural and hyperparameter details provided; code available |
| **Baseline Appropriateness (C2)** | ☑ H | Compared against multiple baselines (BPE, character, word, Morfessor, morphological analyzer) |
| **Evaluation Robustness (C3)** | ☑ H | 3 independent runs; ANOVA, ANCOVA, fixed-effects models with p-values; mean and standard deviation reported |
| **Overall Quality** | ☑ High | Rigorous experimental design with controlled comparisons and statistical analysis |

---

### 10. Reproducibility

| Field | Value |
| :--- | :--- |
| **Code Availability** | ☑ Yes — GitHub repository |
| **Model Availability** | ☑ Yes |
| **Dataset Availability** | ☑ Yes — TeluguMorphScore dataset |
| **Experimental Reproducibility** | ☑ Sufficient details |
| **License** | Not specified |

---

### 11. Reviewer Notes

| Field | Notes |
| :--- | :--- |
| **Methodological Concerns** | Results may not generalize to larger models or decoder-only architectures; limited to NLU tasks |
| **Noteworthy Implementation Details** | 72 models pre-trained; morphological analyzer used for Telugu hybrid tokenizers |
| **Additional Observations** | Strong evidence for Unigram > BPE for agglutinative languages in NLU settings |
| **Information for Narrative Synthesis** | Key paper for RQ3 (typology-sensitive tokenization) and RQ1 (tokenizer comparison) |

---

## File Naming Convention

All extraction files should be saved using the following naming convention:

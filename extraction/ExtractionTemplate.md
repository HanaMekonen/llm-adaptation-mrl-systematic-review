# Standardized Data Extraction Template

This file contains the standardized data extraction template used in the systematic review:

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

## Example Completed Data Extraction Form

# P22 — Vemula et al. (2025)

---

## 1. Study Metadata

| Field | Value |
| :--- | :--- |
| **Paper ID** | P22 |
| **Citation** | Vemula, S. R., Dandapat, S., Sharma, D. M., & Krishnamurthy, P. (2025). *Rethinking Tokenization for Rich Morphology: Morphological Alignment as a Key Factor in Language Modeling*. Proceedings of IJCNLP-AACL 2025 Student Research Workshop. |
| **Publication Year** | 2025 |
| **Publication Type** | Peer-reviewed conference paper |
| **Venue** | IJCNLP-AACL 2025 Student Research Workshop |
| **Publisher** | Association for Computational Linguistics (ACL) |
| **DOI** | 10.18653/v1/2025.ijcnlp-srw.20 |
| **URL** | https://aclanthology.org/2025.ijcnlp-srw.20 |
| **Primary Study** | Yes |
| **Reason for Inclusion** | Investigates tokenizer adaptation for morphologically rich languages through controlled experiments comparing multiple subword segmentation strategies. Directly addresses RQ1, RQ2, and RQ3. |

---

## 2. Research Scope

| Field | Value |
| :--- | :--- |
| **Research Objective** | To investigate how different subword tokenization strategies influence language model performance in morphologically rich languages and whether morphological alignment is a better predictor of downstream performance than vocabulary compression. |
| **Research Domain** | Tokenizer and vocabulary adaptation for morphologically rich languages |
| **Primary Adaptation Category** | Tokenizer adaptation |

---

## 3. Language and Typological Characteristics

| Field | Value |
| :--- | :--- |
| **Languages Investigated** | Telugu, Hindi, English |
| **Primary Target Language** | Telugu |
| **Comparison Languages** | Hindi and English |
| **Language Family** | Telugu – Dravidian; Hindi – Indo-Aryan (Indo-European); English – Germanic (Indo-European) |
| **Writing Systems** | Telugu script, Devanagari, Latin |
| **Morphological Typology** | Telugu – Agglutinative; Hindi – Fusional with moderate agglutinative characteristics; English – Predominantly fusional/analytic |
| **Typology Source** | Established linguistic literature (not explicitly cited by the authors) |
| **Resource Level** | Telugu – Low-resource; Hindi – Medium-resource; English – High-resource |
| **Resource Level Definition** | Not explicitly defined by the authors. Classification inferred from the availability of digital corpora and NLP resources. |
| **Language Roles** | Telugu: primary experimental language; Hindi and English: comparative evaluation languages |

---

## 4. Model Characteristics

| Field | Value |
| :--- | :--- |
| **Base Model** | Custom BERT models trained from scratch |
| **Architecture** | Encoder-only Transformer |
| **Training Objective** | Masked Language Modeling (MLM) |
| **Model Size** | Approximately 8.5M parameters (excluding embedding layer) |
| **Model Availability** | Open-weight |
| **Pretrained Model Used** | No (models trained from scratch) |

---

## 5. Adaptation Strategy

| Field | Value |
| :--- | :--- |
| **Adaptation Category** | Tokenizer/Vocabulary adaptation |
| **Continued Pretraining** | No |
| **Instruction Tuning** | No |
| **Parameter-Efficient Fine-Tuning (PEFT)** | Not used |
| **Prompting** | Not applicable |
| **Tokenizer Methods Compared** | Word-level, Character-level, BPE, Unigram, Morfessor+BPE, Morphological Analyzer+BPE |
| **Morphology-aware Tokenization** | Yes |
| **Vocabulary Sizes Evaluated** | 8K, 16K, and 50K tokens |
| **Vocabulary Expansion** | Not performed; tokenizer variants trained independently |
| **Retrieval-Augmented Generation** | Not applicable |
| **Hybrid Adaptation Pipeline** | Morfessor+BPE and Morphological Analyzer+BPE |

---

## 6. Training Configuration

| Field | Value |
| :--- | :--- |
| **Training Corpus** | WMT News Crawl and IndicCorp |
| **Training Data Size** | Approximately 10 million sentences per language |
| **Data Sources** | IndicCorp, WMT News Crawl |
| **Training Hardware** | NVIDIA RTX 6000 (pretraining); 4 × RTX 2080 GPUs (fine-tuning) |
| **GPU Memory** | Approximately 50 GB VRAM during pretraining |
| **Training Parameters** | Approximately 8.5M trainable parameters |
| **Training Duration** | 175,000 optimization steps |
| **Missing Information** | GPU hours not reported |

---

## 7. Evaluation

| Field | Value |
| :--- | :--- |
| **Evaluation Type** | Discriminative |
| **Tasks** | Text Classification, POS Tagging, Named Entity Recognition, Dependency Parsing, Natural Language Inference, Semantic Textual Similarity |
| **Benchmarks** | IndicGLUE, IndicXTREME, GLUE |
| **Metrics** | Accuracy, F1-score, LAS, Pearson correlation, Spearman correlation, MorphScore |
| **Baselines** | Character tokenizer, Word tokenizer, BPE, Morfessor tokenizer, Morphological Analyzer tokenizer |
| **Experimental Runs** | Three independent runs per experiment |
| **Statistical Analysis** | ANOVA, ANCOVA, fixed-effects regression models, p-values, mean ± standard deviation |

---

## 8. Main Findings

| Field | Value |
| :--- | :--- |
| **Principal Findings** | Morphological alignment is a stronger predictor of downstream performance than traditional token compression measures. Unigram tokenization consistently outperformed BPE for Telugu across most NLP tasks. Hybrid morphology-aware tokenizers improved BPE but did not consistently outperform Unigram. |
| **Key Quantitative Results** | MorphScore (Telugu): Unigram = 0.79, BPE = 0.27. Word similarity improved from approximately 79.7% (BPE) to 89.4% (Unigram). Positive correlation observed between MorphScore and syntactic downstream tasks. |
| **Computational Efficiency** | More than 70 pretrained models and over 2,000 downstream fine-tuning experiments conducted. |
| **Authors' Limitations** | Limited to relatively small encoder models; experiments focus on NLU tasks rather than generative LLMs. |

---

## 9. Contribution to the Review

| Research Question | Contribution |
| :--- | :--- |
| **RQ1** | Demonstrates that tokenizer design is an effective adaptation strategy for morphologically rich languages. |
| **RQ2** | Provides extensive quantitative comparisons across tokenizer families, vocabulary sizes, and downstream tasks. |
| **RQ3** | Strong evidence that morphological typology directly influences tokenizer effectiveness, particularly for agglutinative languages such as Telugu. |
| **RQ4** | Illustrates rigorous evaluation methodology using multiple benchmarks and statistical validation but does not introduce new evaluation metrics or datasets. |

---

## 10. Quality Assessment

| Criterion | Rating | Justification |
| :--- | :--- | :--- |
| **Reporting Clarity** | High (5/5) | Experimental setup, tokenizer construction, datasets, hyperparameters, and implementation details are comprehensively documented. |
| **Baseline Appropriateness** | High (5/5) | Multiple strong baselines representing word-, character-, statistical-, and morphology-aware tokenization are compared under controlled conditions. |
| **Evaluation Robustness** | High (5/5) | Large-scale evaluation across multiple benchmark suites with repeated runs and appropriate statistical significance testing. |
| **Overall Quality** | **15/15 (High)** | High methodological rigor and reproducibility with comprehensive empirical evaluation. |

---

## 11. Reproducibility Assessment

| Field | Value |
| :--- | :--- |
| **Source Code** | Available |
| **Pretrained Models** | Available |
| **Datasets** | Publicly available |
| **Experimental Settings** | Sufficiently documented for replication |
| **License** | Not specified |

---

## 12. Reviewer's Analytical Notes

| Field | Notes |
| :--- | :--- |
| **Methodological Strengths** | Carefully controlled tokenizer comparison while holding model architecture constant; rigorous statistical validation; extensive experimental coverage. |
| **Methodological Weaknesses** | Findings are based on relatively small encoder models and may not transfer directly to contemporary decoder-only LLMs such as LLaMA or Gemma. |
| **Importance for This Review** | One of the strongest empirical studies supporting morphology-aware tokenization. Provides high-quality evidence that morphological typology should inform tokenizer design for low-resource languages. |
| **Evidence Weight** | **High** |
| **Recommended Citation Use** | Background (tokenization), Results (RQ1), Comparative Analysis (RQ2), Typology Discussion (RQ3). |

---

## License

These materials are shared under the Creative Commons Attribution 4.0 International (CC BY 4.0) license.

**Citation:**

> H. Mekonen, "Techniques for Adapting Large Language Models to Low-Resource, Morphologically Rich Languages: A Systematic Review," Seminar II, Addis Ababa University, 2026.

# Standardized Data Extraction Template

**Appendix D: Data Extraction Template for Systematic Review**

**Review Title:** Techniques for Adapting Large Language Models to Low-Resource, Morphologically Rich Languages: A Systematic Review

**Reviewer:** Hana Mekonen

**Date:** [1/7/26]

---

## Instructions for Use

1. **Complete one extraction form per included study.**
2. **Use the paper's full text** (not just the abstract) to extract information.
3. **For missing information**, explicitly note **"Not reported"** in the field.
4. **For information not applicable**, explicitly note **"Not applicable"** in the field.
5. **For estimated values** (e.g. derived from other reported information), explicitly note **"Estimated"** in the field.
6. **Save each extraction** using the naming convention: `P[PaperID]_[FirstAuthor]_[Year].md`
   - Example: `P22_Vemula_2025.md`

---

## Extraction Form

### 1. Study Metadata

| Field | Value |
| :--- | :--- |
| **Paper ID** | [P01–P30] |
| **Authors** | [Full author names] |
| **Year** | [Publication year] |
| **Publication Type** | [Journal article / Conference paper / Workshop paper] |
| **Venue** | [Journal or conference name] |
| **DOI** | [Digital Object Identifier if available] |

---

### 2. Language and Typological Characteristics

| Field | Value |
| :--- | :--- |
| **Target Language(s)** | [All languages investigated] |
| **Language Family** | [e.g., Afroasiatic, Indo-European, Dravidian, Turkic, Austronesian] |
| **Writing System / Script** | [e.g., Latin, Ge'ez, Arabic, Devanagari, Cyrillic, Telugu] |
| **Morphological Typology** | [Agglutinative / Fusional / Non-concatenative / Polysynthetic / Analytic / Isolating / Mixed] |
| **Typology Source** | [WALS / Glottolog / Ethnologue / Established linguistic literature / Study's own characterization / Other] |
| **Resource Level** | [High-resource / Medium-resource / Low-resource] |
| **Resource Level Definition** | [Definition of resource scarcity adopted by the study, if explicitly reported] |
| **Language Role** | [Source / Target / Evaluation / Multilingual / Multiple roles] |

---

### 3. Model Characteristics

| Field | Value |
| :--- | :--- |
| **Base Model** | [e.g., LLaMA, Gemma, Qwen, GPT, BLOOM, mT5, XLM-R, BERT] |
| **Model Size** | [Number of parameters, e.g., 560M, 7B, 13B, 70B] |
| **Model Availability** | [Open-weight / Proprietary API] |
| **Architecture** | [Decoder-only / Encoder-only / Encoder-Decoder] |

---

### 4. Adaptation Strategy

| Field | Value |
| :--- | :--- |
| **Training Objective** | [Continued pretraining / Instruction tuning / Causal LM / Masked LM / Sequence-to-Sequence / Other] |
| **Continued Pretraining** | [Yes / No] — [Corpus description if available] |
| **Parameter-Efficient Fine-Tuning (PEFT)** | [LoRA / IA³ / QLoRA / ReFT / Adapters / Other / None] |
| **LoRA** (if applicable) | [Rank (r): __, Alpha (α): __, Target modules: __, Dropout: __] |
| **IA³** (if applicable) | [Rescaling vectors configuration: __] |
| **QLoRA** (if applicable) | [Quantization method: __, Rank (r): __] |
| **ReFT** (if applicable) | [LayerNorm parameters / Classification head / Other: __] |
| **Prompting** | [Zero-shot / Few-shot / Chain-of-Thought / Least-to-Most / Self-Refine / Other / None] |
| **Tokenizer Adaptation** | [BPE / Unigram / WordPiece / Morphology-aware / SKMT / MoVoC / Other / None] |
| **Vocabulary Expansion** | [Yes / No] — [Number of additional tokens: __] |
| **Retrieval-Augmented Generation (RAG)** (if applicable) | [Retriever: __, Generator: __, Retrieval corpus: __] |
| **Hybrid Adaptation Pipeline** | [Description of multi-stage adaptation if applicable] |

---

### 5. Training Configuration

| Field | Value |
| :--- | :--- |
| **Training Corpus** | [Name and description] |
| **Training Data Size** | [Number of documents / sentences / tokens] |
| **Data Source** | [e.g., OSCAR, mC4, Wikipedia, Common Crawl, custom corpus] |
| **GPU** | [GPU model(s) used] |
| **GPU Memory** | [Peak memory usage in MB/GB, if reported] |
| **Model Parameters** | [Total number of model parameters] |
| **Trainable Parameters** | [Number of trainable parameters during adaptation] |
| **Training Time** | [GPU hours or training duration, if reported] |

---

### 6. Evaluation

| Field | Value |
| :--- | :--- |
| **Task** | [Downstream task: e.g., Translation, QA, NER, Sentiment Analysis, Text Classification] |
| **Evaluation Type** | [Generative / Discriminative] |
| **Evaluation Dataset** | [Benchmark dataset names] |
| **Evaluation Metrics** | [e.g., BLEU, chrF, Accuracy, F1, Exact Match, MorphScore, TSI] |
| **Baseline Models** | [Baseline systems used for comparison] |
| **Experimental Runs** | [Number of independent runs, if reported] |
| **Statistical Analysis** | [Variance measures / Confidence intervals / Significance tests / Other] |

---

### 7. Results

| Field | Value |
| :--- | :--- |
| **Main Findings** | [Principal findings reported by the authors] |
| **Limitations** | [Limitations acknowledged by the authors or identified during extraction] |
| **Key Quantitative Results** | [Reported metrics with values] |
| **Computational Cost** | [GPU hours, memory, parameters, if reported] |

---

### 8. Evidence for Research Questions

| RQ | Contribution | Yes/No | Evidence Description |
| :--- | :--- | :--- | :--- |
| **RQ1** | Adaptation techniques and mechanisms | ☐ Yes / ☐ No | |
| **RQ2** | Quantitative comparison (data, compute, performance) | ☐ Yes / ☐ No | |
| **RQ3** | Typology influence on adaptation | ☐ Yes / ☐ No | |
| **RQ4** | Evaluation, benchmarks, and metrics | ☐ Yes / ☐ No | |

---

### 9. Quality Assessment

**Scoring Rubric:**

| Rating | Criteria |
| :--- | :--- |
| **H (High)** | Fully satisfied with detailed, reproducible information |
| **M (Medium)** | Partially satisfied, but some details missing or insufficient |
| **L (Low)** | Not satisfied or insufficiently addressed |

| Criterion | Rating | Justification |
| :--- | :--- | :--- |
| **Reporting Clarity (C1)** | ☐ H / ☐ M / ☐ L | [Justification] |
| **Baseline Appropriateness (C2)** | ☐ H / ☐ M / ☐ L | [Justification] |
| **Evaluation Robustness (C3)** | ☐ H / ☐ M / ☐ L | [Justification] |
| **Overall Quality** | ☐ High / ☐ Medium / ☐ Low | [Synthesis of three criteria] |

---

### 10. Reproducibility

| Field | Value |
| :--- | :--- |
| **Code Availability** | ☐ Yes / ☐ No — [URL if available] |
| **Model Availability** | ☐ Yes / ☐ No — [URL if available] |
| **Dataset Availability** | ☐ Yes / ☐ No — [URL if available] |
| **Experimental Reproducibility** | ☐ Sufficient details / ☐ Insufficient details |
| **License** | [e.g., CC-BY, MIT, Apache, Not specified] |

---

### 11. Reviewer Notes

| Field | Notes |
| :--- | :--- |
| **Methodological Concerns** | |
| **Noteworthy Implementation Details** | |
| **Additional Observations** | |
| **Information for Narrative Synthesis** | |

---

## Completed Example: Vemula et al. (2025)

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

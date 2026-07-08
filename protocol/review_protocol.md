# Review Protocol

## Overview

This repository contains the review protocol for the systematic review:

> *Techniques for Adapting Large Language Models to Low-Resource, Morphologically Rich Languages: A Systematic Review.*

The protocol was developed prior to conducting the literature search. Although it was not prospectively registered in PROSPERO or the Open Science Framework (OSF), it is publicly shared to improve transparency and reproducibility.

---

# 1. Objective

The objective of this systematic review is to identify, compare, and synthesize adaptation techniques for Large Language Models (LLMs) developed for low-resource morphologically rich languages, with particular attention to the interaction between linguistic typology, data availability, computational constraints, and evaluation methodology.

---

# 2. Research Questions

**RQ1.** How can existing LLM adaptation approaches for low-resource morphologically rich languages be systematically categorized according to their adaptation mechanism and target component?

**RQ2.** How do these adaptation strategies compare in terms of training data requirements, computational cost, parameter efficiency, and reported downstream performance?

**RQ3.** How does morphological typology influence the selection and effectiveness of LLM adaptation strategies for low-resource morphologically rich languages?

**RQ4.** What evaluation benchmarks and metrics are used to evaluate adapted Large Language Models for low-resource morphologically rich languages, and what limitations remain in current evaluation practices?

---

# 3. Information Sources

The literature search was conducted using the following bibliographic databases and discipline-specific repositories:

- Scopus
- ScienceDirect
- IEEE Xplore
- ACL Anthology

Backward and forward citation snowballing was additionally performed using highly relevant review papers and seminal studies.

---

# 4. Search Strategy

The search covered publications from **January 2023 to March 2026**.

Search strings combined three conceptual blocks:

1. Large Language Models
2. Adaptation techniques
3. Low-resource and morphologically rich languages

Database-specific search queries are available in the `search/` directory.

---

# 5. Eligibility Criteria

| Criterion | Inclusion | Exclusion |
|-----------|-----------|-----------|
| Topic | LLM adaptation for low-resource morphologically rich languages | High-resource languages only or non-LLM NLP models |
| Study Type | Empirical studies reporting quantitative evaluation | Opinion papers, editorials, theoretical papers |
| Publication | Peer-reviewed journal or conference paper (2023–2026) | Pre-2023 publications used only as background |
| Language | English full text | Non-English or inaccessible papers |

Survey papers were excluded from the primary synthesis but were used for background literature and citation snowballing.

---

# 6. Data Extraction

For each included study the following information was extracted:

- bibliographic information
- language(s)
- linguistic typology
- adaptation technique
- tokenizer
- training data
- computational requirements
- downstream task
- evaluation benchmark
- evaluation metric
- reported performance
- reproducibility information

---

# 7. Quality Assessment

Each study was assessed using three criteria:

- Reporting clarity
- Baseline appropriateness
- Evaluation robustness

Each criterion was rated as:

- High
- Medium
- Low

---

# 8. Synthesis

Because included studies differed substantially in

- languages,
- datasets,
- adaptation methods,
- evaluation metrics,

a quantitative meta-analysis was not appropriate.

Instead, findings were synthesized using thematic narrative synthesis organized around the research questions.

# Review Protocol

# Techniques for Adapting Large Language Models to Low-Resource, Morphologically Rich Languages: A Systematic Review

**Author:** Hana Mekonen  
**Institution:** Addis Ababa University  
**Supervisor:** Dr. Menore Tekeba

---

## 1. Objective

The objective of this systematic review is to identify, categorize, and critically synthesize adaptation techniques for Large Language Models (LLMs) developed for low-resource morphologically rich languages (MRLs). The review examines how adaptation strategies perform under different combinations of linguistic typology, data availability, and computational constraints.

---

## 2. Research Questions

The review addresses the following research questions:

**RQ1.** How can existing LLM adaptation approaches for low-resource morphologically rich languages be systematically categorized according to their adaptation mechanism and target component?

**RQ2.** How do these adaptation strategies compare with respect to training data requirements, computational cost, parameter efficiency, and reported downstream performance?

**RQ3.** How does morphological typology influence the selection and effectiveness of adaptation strategies for low-resource morphologically rich languages?

**RQ4.** What evaluation benchmarks and metrics are used to evaluate adapted Large Language Models for low-resource morphologically rich languages, and what limitations remain in current evaluation practices?

---

## 3. Review Design

This review follows the **PRISMA 2020** reporting guidelines for systematic reviews. The review protocol was developed before the literature search to improve transparency and reproducibility. Although the protocol was not prospectively registered in a public registry (e.g., PROSPERO), all methodological decisions, search strategies, screening records, and extraction forms are documented in this repository.

---

## 4. Search Strategy

### Information Sources

The literature search was conducted using the following bibliographic databases and discipline-specific repositories:

- Scopus
- ScienceDirect
- IEEE Xplore
- ACL Anthology

Backward and forward citation snowballing were subsequently performed to identify additional eligible studies.

### Search Period

- Publication period: January 2023 – March 2026
- Search date: [Insert final search date]

### Search Concepts

The search strategy combined three conceptual blocks:

1. Large Language Models
2. Adaptation techniques
3. Low-resource and morphologically rich languages

The complete database-specific search strings are provided in the `search/` directory.

---

## 5. Eligibility Criteria

| Criterion | Inclusion | Exclusion |
|-----------|-----------|-----------|
| Topic | Studies proposing, evaluating, or analyzing adaptation techniques for Large Language Models or foundation models in low-resource and/or morphologically rich languages | Studies focusing exclusively on high-resource languages or traditional NLP models without LLMs |
| Study Type | Empirical studies reporting implementation details and experimental evaluation | Opinion papers, editorials, theoretical papers without empirical evaluation, and surveys (except for background and snowballing) |
| Publication | Peer-reviewed journal articles and conference papers published from January 2023 onward | Non-peer-reviewed publications and studies published before January 2023 (except foundational background literature) |
| Language | Full-text articles published in English | Non-English publications or studies without accessible full text |

---

## 6. Study Selection

Study selection followed four stages:

1. Identification
2. Duplicate removal
3. Title and abstract screening
4. Full-text eligibility assessment

Reasons for exclusion during the full-text screening stage were recorded in the screening log.

The complete screening records are available in the `screening/` directory.

---

## 7. Data Extraction

For each included study, the following information was extracted:

- Bibliographic information
- Target language(s)
- Language family and morphological typology
- Adaptation strategy
- Base LLM
- Training data characteristics
- Computational requirements
- Evaluation datasets
- Evaluation metrics
- Reported performance
- Reproducibility information
- Reported limitations

The complete extraction template is available in the `extraction/` directory.

---

## 8. Quality Assessment

Methodological quality was assessed using a structured quality assessment framework comprising three dimensions:

- **C1:** Reporting clarity
- **C2:** Experimental design and baseline appropriateness
- **C3:** Evaluation robustness and reproducibility

Each criterion was rated as:

- High
- Medium
- Low

Quality assessment results are available in the `quality/` directory.

---

## 9. Data Synthesis

Given the substantial heterogeneity across studies—including differences in languages, adaptation techniques, evaluation benchmarks, and reported performance metrics—a quantitative meta-analysis was not appropriate.

Instead, evidence was synthesized using a structured narrative synthesis. Studies were grouped according to:

- adaptation mechanism;
- linguistic typology;
- computational requirements;
- data availability; and
- evaluation methodology.

Comparisons focused on identifying common trends, methodological differences, reported trade-offs, and remaining research gaps.

---

## 10. Repository Contents

This repository includes all supplementary materials required to reproduce the review process:

- review protocol;
- database search strategies;
- screening decisions;
- data extraction sheets;
- quality assessment results; and
- supplementary figures, including the PRISMA flow diagram.

These materials are provided to improve the transparency, reproducibility, and reuse of this systematic review.

# A Systematic Mapping Study of Deep Learning for EGFR Mutation Prediction in Lung Adenocarcinoma

**Lead Author:** Aya Alaoui Sossé (Mohammed V University, Rabat, Morocco · DataPathology)  
**Book Series:** *Studies in Computational Intelligence* (SCI, Volume 1311)  
**Publisher:** **Springer, Cham (Springer Nature Switzerland AG)**  
**ISBN:** [`978-3-032-43857-7`](https://link.springer.com/book/9783032438577) (Hardcover) · [`978-3-032-43858-4`](https://link.springer.com/book/9783032438577) (eBook)

---

## 1. Overview & Clinical Motivation

Actionable **Epidermal Growth Factor Receptor (*EGFR*)** mutations are critical biomarkers for targeted tyrosine kinase inhibitor (TKI) therapy in **lung adenocarcinoma (LUAD)**. While molecular testing (NGS / PCR) is the clinical gold standard, high cost, tissue depletion, and long turnaround times limit accessibility—particularly in **low- and middle-income countries (LMICs)**.

Predicting *EGFR* mutational status directly from routine **Hematoxylin and Eosin (H&E) whole-slide images (WSIs)** using deep learning and weakly supervised **Multiple-Instance Learning (MIL)** offers a rapid, cost-effective pre-screening and triage pathway for precision oncology.

---

## 2. Key Contributions of This Study

1. **Systematic Taxonomy of WSI-Based *EGFR* Prediction:** Comprehensive mapping of deep-learning architectures (CNN patch classifiers, Attention-based MIL, Vision Transformers, and Pathology Foundation Models) applied to H&E histopathology in lung adenocarcinoma.
2. **Dataset & Generalization Audit:** Analysis of public (TCGA-LUAD, CPTAC-LUAD) versus private multi-institutional cohorts, highlighting severe gaps in external validation and demographic diversity.
3. **End-to-End WSI Pipeline Engineering:** Informed the design of our end-to-end *EGFR* prediction pipeline at **DataPathology**, which outperformed baseline benchmark solutions by **+15%** and achieved **94% benchmark accuracy** on mutation prediction from whole-slide images.

---

## 3. End-to-End Computational Pathology Pipeline for Mutation Prediction

```text
[ Gigapixel H&E WSI ]
         │
         ▼
[ Tissue Segmentation & Patch Tiling (20x / 40x) ]
         │
         ▼
[ Stain Normalization & Pathology Foundation Feature Extraction ]
         │
         ▼
[ Attention-Based Multiple-Instance Learning (MIL) Aggregation ]
         │
         ▼
[ Slide-Level EGFR Mutation Probability + Spatial Attention Heatmap ]
```

---

## 4. Official Springer Citation (BibTeX)

```bibtex
@incollection{alaouisossee2027egfr,
  author    = {Alaoui Soss{\x27e}, Aya and others},
  title     = {A Systematic Mapping Study of Deep Learning for {EGFR} Mutation Prediction in Lung Adenocarcinoma},
  booktitle = {Modern Artificial Intelligence and Data Science 2026: Tools, Techniques and Systems},
  editor    = {Idrissi, Abdellah},
  series    = {Studies in Computational Intelligence},
  volume    = {1311},
  publisher = {Springer Nature Switzerland AG},
  address   = {Cham},
  year      = {2027},
  isbn      = {978-3-032-43857-7},
  url       = {https://link.springer.com/book/9783032438577}
}
```

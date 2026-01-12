# Machine Learning-Based Classification & Feature Identification for Psoriasis
### MSc Data Science | Dissertation | NYHDIF Prize Winner | Grade: 86%

## 🎯 Research Aims
The primary goal of this research was to evaluate the effectiveness of supervised machine learning for the classification of psoriasis and the identification of diagnostic biomarkers. 

The project specifically addressed the **"multiplicity problem"** – a phenomenon where different, equally accurate models identify divergent feature sets. By resolving this divergence, the study sought to isolate a consistent, high-confidence gene signature from high-throughput RNA-sequencing data.

---

## 🛠️ Methodology & Frameworks
* **Explainable AI (XAI):** Expert implementation of **SHAP (Tree and Kernel Explainers)** to move beyond "black-box" predictive accuracy and uncover underlying global feature importance.
* **Multi-Model Framework:** Engineered and optimised three methodologically distinct models: **Logistic Regression (LR)**, **Random Forest (RFC)**, and **Support Vector Machines (SVM)**.
* **Data Engineering:**
    * Processed the **NCBI GEO GSE54456** dataset (174 samples; 21,510 genes).
    * Applied **$log_{2}(RPKM + 1)$** transformation to stabilise variance and mitigate right-skewness.
    * Utilised **Variance-Based Selection** to manage the $n \ll P$ problem, retaining the top 5,000 most variable genes.
* **Methodological Rigour:** Restructured the pipeline to ensure variance-based selection was fitted only on training data, successfully preventing **data leakage** and ensuring the scientific validity of the results.



## 🧬 Clinical Perspective & Interpretability
Drawing on **17 years of diagnostic intuition**, I prioritised interpretability to ensure that machine learning outputs align with biological reality:
* **Consensus Modelling:** Engineered a **Consensus Score** (range 0–5) to consolidate feature importance across five distinct analytical methods (LR coefficients, RFC importance, and SHAP values for all models).
* **Diagnostic Integrity:** Leveraged experience in high-dimensional signal interpretation to ensure that machine learning results align with clinical pathophysiology rather than mathematical artefacts.
* **Addressing Multiplicity:** Demonstrated that while all models achieved perfect performance, they identified different "important" genes. Resolving this via XAI is essential for identifying stable biomarkers that can be verified against clinical literature.



---

## 📈 Results & Visualisations
1. **Perfect Classification:** All optimised models achieved an **Area Under the Curve (ROC-AUC) of 1.0000** on the independent test set.
2. **Literature-Validated Signature:** Successfully isolated a five-gene consensus signature (*BTC*, *CHI3L2*, *LCE3A*, *S100A9*, *SPRR2G*) strongly corroborated by existing biological and clinical literature.
3. **Primary Biomarker Identification:** Identified *AKR1B10* as a primary biomarker, providing clear, interpretable evidence of its functional role in keratinocyte overproliferation.



---

## 📁 Repository Structure
* **`code/pre-processing.ipynb`**: Notebook for data loading, inspection, $log_{2}$ transformation, variance-based gene selection, and scaling.
* **`code/model_training_evaluation.ipynb`**: Notebook for model training, hyperparameter tuning, SHAP analysis, and quantitative overlap quantification.
* **`data/Psoriasis_disease_GSE54456_RPKM.csv`**: The primary expression matrix utilised for the primary analysis.
* **`report/Robert-Jacques-Psoriasis-Dissertation.pdf`**: Final prize-winning research report.

---

## 🚀 Reproducibility
The analysis is designed for full environmental replication via **Python 3.13.5**:
1. Clone this repository.
2. Install dependencies via **`requirements.txt`** (including `scikit-learn 1.7.0` and `shap 0.48.0`).
3. Run the notebooks sequentially to regenerate the **Consensus Score** rankings, confusion matrices, and **SHAP summary plots**.

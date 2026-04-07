# 🧠 TEKNOFEST 2026 – AI in Health Competition

> **PSR-MoE: A Mixture of Experts Architecture for Psychiatric Symptom Recognition**
> Submitted to the TEKNOFEST 2026 Artificial Intelligence in Health category.

---

## 📌 Project Overview

This project develops an AI system for ** "early detection of psychiatric disorders" ** using a **Mixture of Experts (MoE)** architecture.

The model learns meaningful patterns from clinical data to perform **benign- patigenic**. A SHAP-based explainability module makes the predictions interpretable for clinicians.

---

## 🎯 Motivation

- Limitations of current approaches and the opportunities AI offers in this domain
- The societal impact of this solution within the TEKNOFEST framework

---

## 🗂️ Repository Structure

```
TEKNOFEST-2026-AI-in-Health/
│
├── teknofestArch_final.ipynb          # Main model architecture & training code
├── PSR_MoE_V2_Teknofest2026.docx      # Technical report (V2)
├── 2026_Sağlıkta_Yapay_Zeka_PSR-      # TEKNOFEST official project submission form
│   Üniversite_ve_Üzeri_lt7Hv.docx
└── README.md
```

---

## 🧬 Model Architecture

### PSR-MoE (Psychiatric Symptom Recognition – Mixture of Experts)

The model consists of the following components:

- **Gating Network:** Dynamically selects which expert(s) to activate based on input features
- **Expert Networks:** PyTorch-based MLP sub-models combined with CatBoost gradient boosting
- **Aggregation Layer:** Weighted combination of expert outputs to produce the final prediction
- **SHAP Explainer:** Provides both local and global model interpretability for clinical transparency

---

## 📊 Dataset

| Attribute | Details |
|-----------|---------|
| Data Source | ClinVAR, genomAD, dbNSFP |
| Number of Samples | Raw : 1 billion, final dataset : 16357 |
| Number of Features | 66 but we used 12 feature |
| Target Variable | Clinical Sig. |
| Train / Test Split | 80 train - 20 test % |

---

## ⚙️ Installation & Usage

### Requirements

```bash
pip install torch numpy pandas catboost shap scikit-learn matplotlib
```

Or using a requirements file:

```bash
pip install -r requirements.txt
```

### Running the Project

1. Clone the repository:

```bash
git clone https://github.com/karanacakoglu/TEKNOFEST-2026-AI-in-Health.git
cd TEKNOFEST-2026-AI-in-Health
```

2. Launch the notebook:

```bash
jupyter notebook teknofestArch_final.ipynb
```

3. Execute the cells in order.

---

## 📈 Results

| Metric | Value |
|--------|-------|
| Accuracy | 93 % |
| F1-Score | 96.121 % |
| AUC-ROC | [0.99 % |
| Precision |  |
| Recall | maximum |

> [PLACEHOLDER: Add comparison baseline if available]

---

## 🔍 Explainability (XAI)

Using **SHAP (SHapley Additive exPlanations)**, the model's decision-making process is visualized to ensure clinical transparency.

- **Global Explanations:** Feature importance summary plots
- **Local Explanations:** Per-prediction waterfall and force plots

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Primary language |
| PyTorch | Deep learning model |
| CatBoost | Gradient boosting expert model |
| SHAP | Explainability |
| NumPy / Pandas | Data processing |
| Matplotlib / Seaborn | Visualization |

---

## 👥 Team

| Name | Role |
|------|------|
| Murat Karanacakoğlu | [PLACEHOLDER: Project Architecture Lead / ML-DL Engineer, Researcher] |
| Efe Karameşe | [Dataset Lead, Data Science Expert] |

**Institution:** Ankara University - Computer Science - Faculty of Science

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 📬 Contact

- GitHub: [@karanacakoglu](https://github.com/karanacakoglu)
- Email: mkaranacak52@gmail.com

---

<p align="center">
  <strong>TEKNOFEST 2026 – Artificial Intelligence in Health</strong><br>
  🇹🇷 Artificial intelligence for Turkey's future
</p>

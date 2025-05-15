## 📚 Literature Review

This section summarizes previous research related to histopathological image analysis using deep learning for cancer detection and classification.

---

### 🔹 Source 1: [Accurate and reproducible invasive breast cancer detection in whole-slide images: A Deep Learning approach for quantifying tumor extent](https://www.nature.com/articles/srep46450#Tab4)

- **Objective**: Develop a deep learning method to detect invasive tumor regions in pathology slides.
- **Methods**: A convolutional neural network (CNN) was trained on 400 annotated WSIs and validated on 200 additional cases from The Cancer Genome Atlas.
- **Outcomes**: Achieved a Dice coefficient of **75.86%**, with a **positive predictive value of 71.62%** and **negative predictive value of 96.77%**.
- **Relation to the Project**: Demonstrates CNNs’ effectiveness in cancer region identification on WSIs—applicable for classifying colon polyps as benign or malignant.

---

### 🔹 Source 2: [Deep learning in cancer genomics and histopathology](https://genomemedicine.biomedcentral.com/articles/10.1186/s13073-024-01315-6)

- **Objective**: Review deep learning applications in histopathology and genomics for cancer diagnosis and prognosis.
- **Methods**: Explores CNNs, Vision Transformers (ViTs), weak/strong supervision, and MIL techniques.
- **Outcomes**: DL models can achieve high performance across tasks (classification, mutation prediction, survival modeling) but require attention to bias and generalization issues.
- **Relation to the Project**: Informs the selection of appropriate architectures (e.g., MIL, ViTs) and supervision strategies for colon polyp classification.

#### 🧠 Technology Comparison

| **Model / Technique**        | **Advantages**                                              | **Relevant Applications**                                                 |
|-----------------------------|-------------------------------------------------------------|---------------------------------------------------------------------------|
| **CNNs**                    | Captures hierarchical features from images                  | Tumor detection, grading, subtype classification                         |
| **Weakly Supervised DL**    | Scalable without manual annotations                         | Slide-level classification, mutation prediction, survival prediction     |
| **Strong Supervision**      | Accurate learning from detailed expert labels               | Tumor delineation, cell-type identification                              |
| **Multiple Instance Learning (MIL)** | Learns from slide-level labels; robust to noisy labels    | Efficient tumor detection; sometimes outperforms strong supervision      |
| **Transformer Models**      | Attention mechanisms for long-range dependencies            | Prognosis and survival modeling; can outperform CNNs                     |
| **Vision Transformers (ViTs)** | Global image context; SOTA in image classification          | Survival prediction from histology images                                |
| **Feature Extraction**      | Reduces dimensionality; works on smaller datasets           | Morphological biomarker prediction                                       |

---

### 🔹 Source 3: [A Petri Dish for Histopathology Image Analysis (MHIST Dataset)](https://arxiv.org/pdf/2101.12355)

- **Objective**: Present a curated dataset for colorectal polyp classification using DL.
- **Methods**: Compiled 3,152 image tiles (224×224 px) from 328 WSIs of hyperplastic polyps (HPs) and sessile serrated adenomas (SSAs), anonymized and verified for quality.
- **Outcomes**: MHIST serves as a benchmark dataset for training and evaluating deep learning models in histopathology.
- **Relation to the Project**: Provides a directly relevant dataset for developing and testing computer vision models to distinguish benign from malignant colon polyps.

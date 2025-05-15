# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: [Accurate and reproducible invasive breast cancer detection in whole-slide images: A Deep Learning approach for quantifying tumor extent]

  - **[Link](https://www.nature.com/articles/srep46450#Tab4)**
  - **Objective**: Evaluate the accuracy and robustness of a deep learning-based method to automatically identify the extent of invasive tumor on digitized images
  - **Methods**: A convolutional neural network for detecting presence of invasive tumor on whole slide images. Our approach involves training the classifier on nearly 400 exemplars from multiple different sites, and scanners, and then independently validating on almost 200 cases from The Cancer Genome Atla
  - **Outcomes**: Our approach yielded a Dice coefficient of 75.86%, a positive predictive value of 71.62% and a negative predictive value of 96.77% in terms of pixel-by-pixel evaluation compared to manually annotated regions of invasive ductal carcinoma.
  - **Relation to the Project**:

- **Source 2**: [Deep learning in cancer genomics and histopathology]

  - **[Link](https://genomemedicine.biomedcentral.com/articles/10.1186/s13073-024-01315-6)**
  - **Objective**: In this review, we summarize current and emerging applications of DL in histopathology and genomics, including basic diagnostic as well as advanced prognostic tasks. 
  - **Methods**: Based on a growing body of evidence, we suggest that DL could be the groundwork for a new kind of workflow in oncology and cancer research. However, we also point out that DL models can have biases and other flaws that users in healthcare and research need to know about, and we propose ways to address them.
  - **Outcomes**:
    
| **Technology / Model**                  | **Advantages**                                                       | **Uses / Applications**                                                                 |
|----------------------------------------|----------------------------------------------------------------------|------------------------------------------------------------------------------------------|
| **Convolutional Neural Networks (CNNs)** | Extract hierarchical features from image data effectively.           | - Tumor detection  <br> - Histological grading  <br> - Tumor subtype classification       |
| **Weakly Supervised DL**               | Eliminates need for manual annotations; highly scalable.              | - Slide-level classification  <br> - Mutation prediction  <br> - Survival prediction     |
| **Strongly Supervised DL**             | Precise learning from manually annotated regions.                     | - Tumor delineation  <br> - Cell type detection                                           |
| **Multiple Instance Learning (MIL)**   | Leverages weak labels efficiently; robust to annotation noise.        | - Slide-level tumor detection  <br> - Outperforms some strongly supervised models         |
| **Transformer Neural Networks**        | Uses attention mechanisms to focus on relevant features; efficient.   | - Prognosis prediction  <br> - Survival modeling  <br> - Often outperforms CNNs          |
| **Vision Transformers (ViTs)**         | Superior image-level context capture; state-of-the-art performance.   | - Predicting patient survival from histology images                                       |
| **Feature Extraction Methods**         | Reduces dimensionality; supports downstream modeling on large data.   | - Predicting morphological biomarkers  <br> - Integration with clinical/genomic data     |


  - **Relation to the Project**:

- **Source 3**: [A Petri Dish for Histopathology Image Analysis]

  - **[Link](https://arxiv.org/pdf/2101.12355)**
  - **Objective**: We use MHIST to study natural
questions such as how dataset size, network depth, transfer learning, and high-disagreement examples affect model
performance.
  - **Methods**: For our dataset, we scanned 328 Formalin Fixed
Paraffin-Embedded (FFPE) whole-slide images of colorectal polyps, which were originally diagnosed on the wholeslide level as hyperplastic polyps (HPs) or sessile serrated adenomas (SSAs), from patients at the DartmouthHitchcock Medical Center. These slides were scanned by
an Aperio AT2 scanner at 40x resolution; to increase the
field of view, we compress the slides with 8x magnification. From these 328 whole-slide images, we then extracted
3,152 image tiles (portions of size 224 × 224 pixels) representing diagnostically-relevant regions of interest for HPs
or SSAs. These images were shuffled and anonymized by
removing all metadata such that no sensitive patient information was retrievable from any images. All images contain
mostly tissue by area (as opposed to white space) and were
confirmed by our pathologists to be high-quality with few
artifacts. The use and release of our dataset was approved
by Dartmouth-Hitchcock Health IRB
  - **Outcomes**:
  - **Relation to the Project**: In this paper, we aim to have provided a dataset that can
serve as a petri dish for histopathology image analysis. We
hope that researchers are able to use MHIST to test models
on a smaller scale before being implemented in large-scale
applications, and that our dataset will facilitate further research into deep learning methodologies for histopathology
image analysis.

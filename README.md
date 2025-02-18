# Multi-Branch CNN-LSTM Fusion Network-Driven System with BERT Semantic Evaluator for Radiology Reporting in Emergency Head CTs

This repository contains the source code of our **multi-branch CNN-LSTM fusion network-driven system**, developed for *automatic radiology reporting* from head CT scans of emergency room patients.  

For more details, please *refer to our related publication*:


> **Tomassini, S., Duranti, D., Zeggada, A., Quattrocchi, C. C., Melgani, F., & Giorgini, P.** (2025). *Multi-Branch CNN-LSTM Fusion Network-Driven System with BERT Semantic Evaluator for Radiology Reporting in Emergency Head CTs*. **IEEE Journal of Translational Engineering in Health and Medicine**. DOI: 10.1109/JTEHM.2025.3535676.

---

# Abstract

**Background and objective**: The high volume of emergency room patients often necessitates head CT examinations to rule out ischemic, hemorrhagic, or other organic pathologies. A system that enhances the diagnostic efficacy of head CT imaging in emergency settings through structured reporting would significantly improve clinical decision making. Currently, no AI solutions address this need. Thus, our research aims to develop an automatic radiology reporting system by directly analyzing brain anomalies in head CT data. 
**Data and methodology**: We propose a multi-branch CNN-LSTM fusion network-driven system for enhanced radiology reporting in emergency settings. We preprocessed head CT scans by resizing all slices, selecting those with significant variability, and applying PCA to retain 95% of the original data variance, ultimately saving the most representative five slices for each scan. We linked the reports to their respective slice IDs, divided them into individual captions, and preprocessed each. We performed an 80-20 split of the dataset for ten times, with 15% of the training set used for validation. Our model utilizes a pretrained VGG16, processing groups of five slices simultaneously, and features multiple end-to-end LSTM branches, each specialized in predicting one caption, subsequently combined to form the ordered reports after a BERT-based semantic evaluation. 
**Results and discussion**: Our system demonstrates effectiveness and stability, with the postprocessing stage refining the syntax of the generated descriptions. However, there remains an opportunity to empower the evaluation framework to more accurately assess the clinical relevance of the automatically-written reports. Part of future work will include transitioning to 3D and developing an improved version based on vision-language models.

# Data & Code

- **Data**: Raw data are *private* due to patient confidentiality and cannot be shared.  
- **Code**: Full code is *available* upon request.

For more information, please *contact the corresponding author*.  

# Requirements
- **Python**: 3.10+  
- **TensorFlow**: 2.15+  
- **Memory**: 24 GB RAM / 40 GB VRAM or higher  
- **GPU Compatibility**:  
  - NVIDIA A100 *(tested)*  
  - NVIDIA GEFORCE RTX 4080 *(tested)*  

# Terms of use
If you use this code (or part of it) in your research, please *cite the original paper*.  

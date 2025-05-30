# Skin-Cancer-Detection-using-Multimodal-RAG
</br>


This project implements an Agentic Multimodal Retrieval-Augmented Generation (RAG) framework designed for interactive medical image analysis, specifically focused on skin cancer diagnosis. Combining state-of-the-art deep learning, CLIP-based visual-language alignment, and retrieval-based reasoning, the system offers interpretable, context-aware diagnostic reports and supports interactive clinical dialogue.
</br>



  
## 🔍 Overview
Modern healthcare demands not just high-accuracy AI diagnostics but systems that are explainable and interactive. This project builds a system that:

- Analyzes dermatoscopic images using a CNN-based visual extractor.
- Selects clinically significant features via a novel DAA-Deep module.
- Aligns visual and textual data using CLIP embeddings.
- Generates diagnostic reports and enables interactive Q&A using RAG.

Validated on the HAM10000 dataset, our system demonstrates state-of-the-art performance in both diagnostic accuracy and explainability.
</br>



## 🧠 Key Features
| Component  | Description  |
| ------------- | ------------- |
| 🧠 DAA-Deep  | Confidence-based differential feature selector for improved precision  |
| 📷 Visual Extractor  | Deep CNN (e.g., ResNet50) for skin lesion feature extraction  |
| 🔗 CLIP Embeddings  | Aligns image features with medical text for semantic relevance |
| 📚 RAG Module  | Retrieves and generates human-readable diagnostic reports |
| 💬 Interactive Dialogue  | Clinician-like follow-up Q&A to clarify diagnoses  |
</br>


## 📊 Results (HAM10000 Dataset)
| Model Config  | Accuracy | ROUGE-L | Q&A Score | 
| ------------- | ------------- | --------- | ------ |
| Full System (DAA + CLIP + RAG) | 88.5 ± 1.2 | 0.65 ± 0.05 | 4.2 ± 0.6 |
| Without DAA | 82.3 ± 1.5 | - | - |
| Without CLIP  | 88.5 ± 1.2 | 0.50 ± 0.04 | 3.1 ± 0.7 |


## Flow Diagram
![image](https://github.com/user-attachments/assets/a00e0fe1-5b61-4e6d-b843-89b50de769ba)



# Translate With Care (TWC)


This repository contains the official implementation of the paper:

**Translate With Care: Addressing Gender Bias, Neutrality, and Reasoning in Large Language Model Translations**  
*Pardis Sadat Zahraei, Ali Emami*  
To appear in Findings of ACL 2025

---

## 🧠 Overview

Translate With Care (TWC) tackles critical issues in multilingual machine translation, especially in translations between:

- **Genderless languages** (e.g., Persian, Indonesian, Finnish)  
- **Natural gender languages** (e.g., English)

The focus is on three key challenges:

1. **Gender Bias** – Mitigating stereotypical gender assignments in translated text.
2. **Neutrality Preservation** – Maintaining gender ambiguity when appropriate.
3. **Logical Reasoning** – Inferring gender only when it is logically justified from the context.

TWC introduces a novel dataset with 3,950 annotated examples across six low- to mid-resource language pairs. Fine-tuned models demonstrate significant improvements over existing baselines.

---

## 📁 Repository Structure

```
📁 Repository Root
├── TWC_Dataset_Generation_+_Evaluation.ipynb   # Notebook for dataset generation and evaluation
├── Finetune.ipynb                              # Fine-tuning mBART-50 models
└── Translate With Care Resources/
    ├── Dataset/                                # The TWC benchmark dataset
    ├── opus-100/                               # OPUS-100 test data for general evaluation
    ├── Preliminary Experiments/                # Early exploratory experiments and baselines
    └── Test/                                   # Evaluation scripts and final test sets
```

---

## 📦 Dataset

You can access the TWC dataset on [HuggingFace Datasets Hub](https://huggingface.co/datasets/PardisSzah/TWC).

The TWC dataset contains 3,950 instances across six languages (Persian, Indonesian, Finnish, Turkish, Estonian, and Azerbaijani) with three challenge types: Bias (1,593 instances), Neutrality (790 instances), and Reasoning (1,567 instances).

---


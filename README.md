# mBERT Optimization for Multilingual Recommendation Engines
**Addressing the Multilingual Bottleneck via Dynamic Optimization and Hybrid Loss Strategies**

![Thesis](https://img.shields.io/badge/Thesis-MS_Computer_Science-blue)
![NLP](https://img.shields.io/badge/NLP-mBERT-red)
![Optimization](https://img.shields.io/badge/Optimization-Knowledge_Distillation-yellow)

## 🎯 Overview
This repository showcases the research methodology and architectural frameworks developed for my Master's Thesis: **"Addressing the Multilingual Bottleneck in Recommendation Engines."** The research addresses the conflict between the 177M parameter count of mBERT and the low-latency requirements of real-world recommendation systems.

## 🚀 Key Research Contributions
- **mBERT-Tiny Architecture:** Developed a family of scalable variants (Tiny2, Tiny4, Tiny6) to balance the accuracy-efficiency trade-off.
- **Hybrid Loss Function:** Innovated a training mechanism combining **Cross-Entropy** and **Focal Loss** to maintain stability while addressing class/language imbalance.
- **Latency Reduction:** Achieved a reduction in inference time from standard mBERT (~150ms) down to **6.12ms (Tiny2)** and **25.95ms (Tiny6)**.
- **Parameter Efficiency:** Successfully compressed the model footprint from 177M parameters to as low as **6.2M (Tiny2)** while preserving multilingual transfer capabilities.

## 🛠️ Technical Stack
- **Base Model:** Multilingual BERT (mBERT-base-cased).
- **Optimization:** Dynamic model scaling, Parameter Reduction, and Hybrid Loss formulation.
- **Environment:** AWS SageMaker, PyTorch, Transformers (HuggingFace).
- **Datasets:** Evaluated using IMDB (Sentiment), AG News (Classification), and Synthetic industrial datasets.

## 📊 Evaluation Metrics (Research Highlights)
| Model Variant | Parameters | Latency (CPU) | Key Use-Case |
| :--- | :--- | :--- | :--- |
| **mBERT (Baseline)** | 177M | ~150ms | High-accuracy Cloud |
| **Tiny6** | 28.4M | 25.95ms | Real-time Recommendation |
| **Tiny2** | 6.2M | 6.12ms | Resource-Constrained Edge |

## 📁 Repository Structure
- `notebooks/`: Implementation of the mBERT-Tiny architectural scaling.
- `scripts/`: Custom training loops incorporating the Hybrid Loss function.
- `results/`: Visualization of the Accuracy vs. Latency Pareto front.
- `docs/`: Summary of the "Multilingual Bottleneck" theoretical framework.

## 📚 Publication & Thesis Status
- **Status:** Final Defense Scheduled for **January 2026**.
- **Institution:** Faculty of Computer Science and IT, The Superior University, Lahore.
- **Core Findings:** Demonstrated that targeted parameter reduction can maintain cross-lingual performance while enabling deployment on edge-level hardware.

---
*Note: This repository contains research templates and architectural summaries. Full proprietary datasets and trained weights are restricted pending journal publication.*

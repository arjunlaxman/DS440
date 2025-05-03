# DS440 – Ethereum Smart Contract Vulnerability Detection

This repository contains the final capstone project for DS440W at The Pennsylvania State University. Our goal was to design a scalable, hybrid system for detecting vulnerabilities in Ethereum smart contracts using both deep learning models and static analysis tools.

## 🧠 Project Overview

We combined pretrained transformer models and static analyzers to automatically detect, classify, and even suggest fixes for vulnerabilities in Solidity contracts.

### Key Technologies Used
- **CodeBERT** – for classification of secure vs. vulnerable contracts.
- **GraphCodeBERT** – enhanced detection using data flow graphs.
- **CodeT5+** – added generative capabilities to suggest security patches.
- **Slither** – static analysis for rule-based bug detection (e.g., reentrancy).

### Main Contributions
- Developed a multi-model ML pipeline with token, graph, and generative layers.
- Integrated Slither to catch rule-based issues missed by ML.
- Achieved validation accuracy of up to **77.6%**.
- Detected 29 new bugs missed by standard tools.

## 📂 Notebooks

| File | Purpose |
|------|---------|
| `Project_Main.ipynb` | Full training + evaluation pipeline |
| `3demo-v1.ipynb` | Baseline: CodeBERT |
| `3demo-v2-t5.ipynb` | CodeT5+ with patch suggestion |
| `3demo-v1-wild_apply.ipynb` | Inference on SmartBugs Wild Dataset |

## 📊 Dataset Sources

- [SB Curated](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)
- [Consolidated Ground Truth (CGT)](https://github.com/smartbugs/smartbugs)
- [SmartBugs Wild Dataset](https://github.com/smartbugs/smartbugs)

## 📖 Reference

Essay Reference: [arXiv:1910.10601](https://arxiv.org/abs/1910.10601)  
GitHub: [smartbugs/smartbugs](https://github.com/smartbugs/smartbugs)

---

**Team Members:**
- Dominic Felice  
- Jiaqi Lu  
- Arjun Laxman  
- Jiaxi Li  

May 2025 – DS440W Final Report

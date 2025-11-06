# Exploring the Role of Large Language Models in Network Security

This repository contains the notebooks for the research project  
**“Exploring the Role of Large Language Models in Network Security”**,  
conducted as part of the Master of Computer Science program at the **University of Adelaide (2025)**.

---

## Repository Structure

The repository is organized into clearly defined modules to ensure reproducibility and ease of navigation.
All experiment notebooks are stored in the notebooks/ directory, where each Jupyter notebook corresponds to a specific LLM–classifier combination (e.g., RandomForest_Gemma.ipynb, DecisionTree_GPT2.ipynb, ExtraTrees_LLaMA.ipynb).
The root of the repository includes this README.md for detailed instructions.
This structured layout facilitates straightforward replication of experiments and easy integration into future extensions or collaborative research workflows.

## Overview

This study integrates **Large Language Models (LLMs)** with classical machine learning classifiers to improve network intrusion detection.  
Each network flow is converted into a natural-language summary and embedded using pretrained transformers (GPT-2, Gemma, MiniLM, LLaMA-2, BAAI).  
The resulting semantic embeddings are fused with numeric network features and evaluated using traditional classifiers.

---

## Experimental Setup

All experiments were executed in **Google Colab Pro+ (Tesla T4 GPU, 16 GB VRAM)**  
using **Python 3.12**, **Torch 2.3.1**, **Transformers 4.41**, and **Scikit-learn 1.4**.  

**Environment Configuration:**
| Component | Specification |
|------------|---------------|
| Hardware | Google Colab Pro+ |
| Libraries | Transformers, Scikit-learn, Torch, Pandas, NumPy |
| Tokenization | Hugging Face `AutoTokenizer` |
| Visualization | Matplotlib, Seaborn |

---

## Datasets

| Dataset | Year | Type | Samples | Source |
|----------|------|------|----------|--------|
| **NSL-KDD** | 2009 | TCP/IP Traffic | 148k | University of New Brunswick |
| **UNSW-NB15** | 2015 | Hybrid (Network + Application) | 257k | UNSW Canberra Cyber Range Lab |
| **TON-IoT** | 2020 | IoT + Sensor Network | 461k | CSIRO Data61, Australia |

---

## How to Reproduce

1. Clone this repository:

   a. git clone https://github.com/Tuhin97/Research-Project.git
   
   b. cd Research-Project
3. Authenticate with Hugging Face for Gemma or LLaMA-2:

   a. from huggingface_hub import login
   
   b. login(token="your_hf_token_here")
5. Open any notebook in Jupyter or Colab and run.



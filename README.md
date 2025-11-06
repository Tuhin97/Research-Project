# Exploring the Role of Large Language Models in Network Security

This repository contains all Python notebooks, datasets, and visual results used for the research project  
**“Exploring the Role of Large Language Models in Network Security”**  
conducted by **Tuhin Anand (a1930716)** as part of the **Master of Computer Science (University of Adelaide, 2025)**.

---

## Overview

This project investigates how **Large Language Models (LLMs)** can enhance **network intrusion detection systems (IDS)** by combining  
semantic embeddings from pretrained transformer models — **GPT-2, Gemma, MiniLM, BAAI (bge-base), and LLaMA-2** —  
with traditional classifiers (**Decision Tree**, **Extra Trees**, and **Random Forest**).

The objective is to evaluate whether contextual LLM embeddings improve detection accuracy, recall, and generalization  
across benchmark cybersecurity datasets — **NSL-KDD**, **UNSW-NB15**, and **TON-IoT**.

---

# Exploring the Role of Large Language Models in Network Security

This repository contains the notebooks for the research project  
**“Exploring the Role of Large Language Models in Network Security”**,  
conducted as part of the Master of Computer Science program at the **University of Adelaide (2025)**.

---

## Repository Structure

├── Decision Tree Notebooks/
│ ├── NSL-KDD/ 
│ ├── UNSW/
│ └── TON-IoT/
├── ExtraTree Notebooks/
│ ├── NSL-KDD/
│ ├── UNSW/
│ └── TON-IoT/
├── Random Forest Notebooks/
│ ├── NSL-KDD/
│ ├── UNSW/
│ └── TON-IoT/
│
└── README.md

---

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



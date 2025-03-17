# LLM-KG4QA: Large Language Models and Knowledge Graphs for Question Answering

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) ![](https://img.shields.io/github/last-commit/machuangtao/LLM-KG4QA?color=blue) ![Stars](https://img.shields.io/github/stars/machuangtao/LLM-KG4QA?color=blue)  ![Forks](https://img.shields.io/github/forks/machuangtao/LLM-KG4QA?color=blue&label=Fork)

## 🔔 News
- **`2025-08`** Our [survey](https://machuangtao.github.io/LLM-KG4QA/survey-emnlp25) has been accepted to **[EMNLP2025](https://2025.emnlp.org)** main conference.
- **`2025-05`** The preprint of our survey is avaliable on **[arXiv](https://arxiv.org/abs/2505.20099)**.
- **`2025-02`** Our [tutorial](https://machuangtao.github.io/LLM-KG4QA/tutorial-edbt25) was accepted to be presented at **EDBT2025**.
- **`2024-12`** We create this repository to maintain a paper list on **LLMs and KGs for QA.**

If you find our work is useful,  please cite our paper by using the following BibTeX entry.

```
@inproceedings{ma2025llmkg4qa,
  title={Large Language Models Meet Knowledge Graphs for Question Answering: Synthesis and Opportunities},
  author={Ma, Chuangtao and Chen, Yongrui and Wu, Tianxing and Khan, Arijit and Wang, Haofen},
  booktitle={Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing,{EMNLP}2025},
  year ={2025},
  publisher={Association for Computational Linguistics},
  pages = {24589--24608}
```

## Content
- [LLM and KGs for QA](#1-llms-and-kgs-for-qa)
  - [KGs as Background Knowledge](#kgs-as-background-knowledge)
  - [KGs as Reasoning Guideline](#kgs-as-reasoning-guideline)
  - [KGs as Refiner and Filter](#kgs-as-refiner-and-filter)
  <!--- - [Hybrid Methods](#hybrid-methods) -->
- [Complex QA](#2-complex-qa)
  - [Explainable QA](#explainable-qa)
  - [Multi-modal QA](#multi-modal-qa)
  - [Multi-document QA](#multi-document-qa)
  - [Multi-Hop QA](#multi-hop-qa)
  - [Multi-run and Conversational QA](#multi-run-and-conversational-qa)
  - [Temporal QA](#temporal-qa)
  - [Multi-domain and Multilingual QA](#multi-domain-and-multilingual-qa)
- [Advanced Topics](#3-advanced-topics)
  - [Optimization](#optimization)
  - [Data Management](#data-management)
- [Benchmark and Applications](#4-benchmark-and-applications)
  - [Benchmark Dataset](#benchmark-dataset)
  - [Industrial and Scientific Applications](#industrial-and-scientific-applications)
  - [Demo](#demo)
- [Related Survey](#5-related-survey)
---
## 1. LLMs and KGs for QA

### KGs as Background Knowledge
#### Pre-training and Fine-tuning

| NO | Title                                                                                                        | Venue                                                                                                                                                    | Year | Category                                       |Paper Link                                                                                           |
|----|--------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|------|------------------------------------------------|------------------------------------------------------------------------------------------------|
| 1 | Deep Bidirectional Language-Knowledge Graph pretraining   | NeurIPS | 2022|  Pre-training    | [Link](https://proceedings.neurips.cc/paper_files/paper/2022/file/f224f056694bcfe465c5d84579785761-Paper-Conference.pdf)                             
| 2 | GreaseLM: Graph REASoning Enhanced Language Models    | ICLR    | 2022 |  Pre-training     | [Link](https://openreview.net/forum?id=41e9o6cQPj) 
| 3 | InfuserKI: Enhancing Large Language Models with Knowledge Graphs via Infuser-Guided Knowledge Integration  | LLM+KG@VLDB   | 2024 | Pre-training     | [Link](https://arxiv.org/abs/2402.11441)
| 4 | Large Language Models Meet Knowledge Graphs to Answer Factoid Questions  | PACLIC  | 2023 | Pre-training     | [Link](https://aclanthology.org/2023.paclic-1.63/)
| 5 | KaLM: Knowledge-aligned Autoregressive Language Modeling via Dual-view Knowledge Graph Contrastive Learning  | arXiv    | 2024 | Pre-training     | [Link](https://arxiv.org/abs/2412.04948)
| 6 | KBLaM: Knowledge Base augmented Language Model | ICLR    | 2025 | Pre-training     | [Link](https://openreview.net/forum?id=aLsMzkTej9)
| 7 | KnowLA: Enhancing Parameter-efficient Finetuning with Knowledgeable Adaptation  | NAACL   | 2024 |  Fine-Tuning     | [Link](https://aclanthology.org/2024.naacl-long.396/)
| 8 | KG-Adapter: Enabling Knowledge Graph Integration in Large Language Models through Parameter-Efficient Fine-Tuning  | ACL Findlings  | 2024 | Fine-Tuning     | [Link](https://aclanthology.org/2024.findings-acl.229/) 
| 9 | A GAIL Fine-Tuned LLM Enhanced Framework for Low-Resource Knowledge Graph Question Answering  | CIKM    | 2024 |  Fine-Tuning    | [Link](https://dl.acm.org/doi/10.1145/3627673.3679753)
| 10 | Knowledge Graph Finetuning Enhances Knowledge Manipulation in Large Language Models  | ICLR    | 2025 |  Fine-Tuning    | [Link](https://openreview.net/forum?id=oMFOKjwaRS)
| 11 | KLearn Together: Joint Multitask Finetuning of Pretrained KG-enhanced LLM for Downstream Tasks  | GenAIK@COLING    | 2025 |  Fine-Tuning    | [Link](https://aclanthology.org/2025.genaik-1.2/)
| 12 | Improving Pre-trained Language Models with Knowledge Enhancement and Filtering Framework  | NAACL Findings    | 2025 |  Fine-Tuning    | [Link](https://aclanthology.org/2025.findings-naacl.213/)
| 13 | Prompting Large Language Models with Knowledge Graphs for Question Answering Involving Long-tail Facts  | arXiv       | 2024 |  KG-Augmented Prompting    | [Link](https://arxiv.org/abs/2405.06524)
| 14 | KnowGPT: Knowledge Graph based Prompting for Large Language Models  | arXiv     | 2024 |  KG-Augmented Prompting    | [Link](https://arxiv.org/abs/2312.06185) 
| 15 | Knowledge-Augmented Language Model Prompting for Zero-Shot Knowledge Graph Question Answering  | NLRSE          | 2023 |  KG-Augmented Prompting    | [Link](https://aclanthology.org/2023.nlrse-1.7/)
| 16 | Retrieve-Rewrite-Answer: A KG-to-Text Enhanced LLMs Framework for Knowledge Graph Question Answering | IJCKG    | 2023 |  KG-Augmented Prompting    | [Link](https://ijckg2023.knowledge-graph.jp/pages/proc/paper_30.pdf/)
| 17 | Mitigating LLM Hallucinations with Knowledge Graphs: A Case Study | arXiv    | 2025 |  KG-Augmented Prompting    | [Link](https://arxiv.org/abs/2504.12422/)


#### RAG (Retrieval Augmented Generation)

| NO | Title                                                                                                        | Venue                                                                                                                                                    | Year | Category                                       |Paper Link                                                                                           |
|----|--------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|------|------------------------------------------------|------------------------------------------------------------------------------------------------|
| 1 | Enhancing Textbook Question Answering Task with Large Language Models and Retrieval Augmented Generation| arXiv          | 2024 | RAG   | [Link](https://arxiv.org/abs/2402.05128)
| 2 | Retrieval-enhanced Knowledge Editing in Language Models for Multi-Hop Question Answering | CIKM   | 2024 |  RAG   | [Link](https://dl.acm.org/doi/abs/10.1145/3627673.3679722) 
| 3 | Understand What LLM Needs: Dual Preference Alignment for Retrieval-Augmented Generation | arXiv   | 2024 |  RAG   | [Link](https://arxiv.org/abs/2406.18676) 
| 4 | RAG-based Question Answering over Heterogeneous Data and Text | arXiv   | 2024 |  RAG   | [Link](https://arxiv.org/abs/2412.07420) 
| 5 | Awakening Augmented Generation: Learning to Awaken Internal Knowledge of Large Language Models for Question Answering | COLING   | 2025 |  RAG   | [Link](https://aclanthology.org/2025.coling-main.89/) 
| 6 | SAGE: A Framework of Precise Retrieval for RAG | arXiv   | 2025 |  RAG   | [Link](https://arxiv.org/abs/2503.01713) 
| 7 | From Local to Global: A Graph RAG Approach to Query-Focused Summarization  | arXiv  | 2024 | Graph RAG| [Link](https://arxiv.org/abs/2404.16130)
| 8 | LightRAG: Simple and Fast Retrieval-Augmented Generatio  | arXiv   | 2024 |  Graph RAG | [Link](https://arxiv.org/abs/2410.05779)
| 9 | GRAG: Graph Retrieval-Augmented Generation | arXiv   | 2024 |  Graph RAG    | [Link](https://arxiv.org/abs/2405.16506) 
| 10 | HybGRAG: Hybrid Retrieval-Augmented Generation on Textual and Relational Knowledge Bases | arXiv   | 2024 |  Graph RAG    | [Link](https://arxiv.org/abs/2412.16311) 
| 11 | CG-RAG: Research Question Answering by Citation Graph Retrieval-Augmented LLMs | arXiv   | 2025 |  Graph RAG    | [Link](https://arxiv.org/abs/2501.15067) 
| 12 | MiniRAG: Towards Extremely Simple Retrieval-Augmented Generation | arXiv  | 2025 | Graph RAG | [Link](https://arxiv.org/abs/2501.06713)
| 13 | GFM-RAG: Graph Foundation Model for Retrieval Augmented Generation | arXiv  | 2025 | Graph RAG | [Link](https://arxiv.org/abs/2502.01113)
| 14 | MSG-LLM: A Multi-scale Interactive Framework for Graph-enhanced Large Language Models | COLING  | 2025 | Graph RAG | [Link](https://aclanthology.org/2025.coling-main.648/)
| 15 | PathRAG: Pruning Graph-based Retrieval Augmented Generation with Relational Paths | arXiv  | 2025 | Graph RAG | [Link](https://arxiv.org/abs/2502.14902/)
| 16 | In-depth Analysis of Graph-based RAG in a Unified Framework | arXiv  | 2025 | Graph RAG | [Link](https://www.arxiv.org/abs/2503.04338/)
| 17 | Empowering GraphRAG with Knowledge Filtering and Integration | arXiv  | 2025 | Graph RAG | [Link](https://arxiv.org/abs/2503.13804/)
| 18 | Graph Neural Network Enhanced Retrieval for Question Answering of Large Language Models | NAACL  | 2025 | Graph RAG | [Link](https://aclanthology.org/2025.naacl-long.337/)
| 19 | NodeRAG: Structuring Graph-based RAG with Heterogeneous Nodes | arXiv  | 2025 | Graph RAG | [Link](https://arxiv.org/abs/2504.11544/)
| 20 | KG-RAG: Bridging the Gap Between Knowledge and Creativity | arXiv   | 2024 |  KG RAG   | [Link](https://arxiv.org/abs/2405.12035)
| 21 | Knowledge Graph-extended Retrieval Augmented Generation for Question Answering | arXiv   | 2025 |  KG RAG   | [Link](https://arxiv.org/abs/2504.08893)
| 22 | Retrieval-Augmented Generation with Knowledge Graphs for Customer Service Question Answering| SIGIR         | 2024 | KG RAG    | [Link](https://dl.acm.org/doi/10.1145/3626772.3661370)
| 23 | REnhancing Large Language Models with Knowledge Graphs for Robust Question Answering | ICPADS   | 2024 |  KG RAG    | [Link](https://doi.ieeecomputersociety.org/10.1109/ICPADS63350.2024.00042) 
| 24 | FRAG: A Flexible Modular Framework for Retrieval-Augmented Generation based on Knowledge Graphs | arXiv   | 2025 |  KG RAG    | [Link](https://arxiv.org/abs/2501.09957) 
| 25 | SimGRAG: Leveraging Similar Subgraphs for Knowledge Graphs Driven Retrieval-Augmented Generation | arXiv   | 2025 |  KG RAG    | [Link](https://arxiv.org/abs/2412.15272) 
| 26 | RGR-KBQA: Generating Logical Forms for Question Answering Using Knowledge-Graph-Enhanced Large Language Model | COLING   | 2025 |  KG RAG    | [Link](https://aclanthology.org/2025.coling-main.205) 
| 27 | Knowledge Graph-Guided Retrieval Augmented Generation | arXiv   | 2025 |  KG RAG    | [Link](https://arxiv.org/abs/2502.06864) 
| 28 | Simple Is Effective: The Roles of Graphs and Large Language Models in Knowledge-Graph-Based Retrieval-Augmented Generation | ICLR | 2025 | KG RAG  | [Link](https://openreview.net/forum?id=JvkuZZ04O7) 
| 29 | CoT-RAG: Integrating Chain of Thought and Retrieval-Augmented Generation to Enhance Reasoning in Large Language Models | arXiv | 2025 | KG RAG  | [Link](https://arxiv.org/abs/2504.13534) 
| 30 | A Pilot Empirical Study on When and How to Use Knowledge Graphs as Retrieval Augmented Generation | arXiv | 2025 | KG RAG  | [Link](https://arxiv.org/abs/2502.20854) 
| 31 | A Systematic Exploration of Knowledge Graph Alignment with Large Language Models in Retrieval Augmented Generation | AAAI | 2025 | KG RAG  | [Link](https://ojs.aaai.org/index.php/AAAI/article/view/34716) 
| 32 | Evaluating Knowledge Graph Based Retrieval Augmented Generation Methods under Knowledge Incompleteness | arXiv | 2025 | KG RAG  | [Link](https://arxiv.org/abs/2504.05163) 
| 33 | RAG-KG-IL: A Multi-Agent Hybrid Framework for Reducing Hallucinations and Enhancing LLM Reasoning through RAG and Incremental Knowledge Graph Learning Integration | arXiv | 2025 | KG RAG  | [Link](https://arxiv.org/abs/2503.13514) 
| 34 | Empowering LLMs by hybrid retrieval-augmented generation for domain-centric Q&A in smart manufacturing | Advanced Engineering Informatics | 2025| Hybrid RAG  | [Link](https://doi.org/10.1016/j.aei.2025.103212) 
| 35 | Spatial-RAG: Spatial Retrieval Augmented Generation for Real-World Spatial Reasoning Questions | arXiv | 2025 | Spatial RAG  | [Link](https://arxiv.org/abs/2502.18470) 
| 36 | Spatial-RAG: Spatial Retrieval Augmented Generation for Real-World Spatial Reasoning Questions | arXiv | 2025 | Spatial RAG  | [Link](https://arxiv.org/abs/2502.18470) 

### KGs as Reasoning Guideline

| NO | Title                                                                                                        | Venue                                                                                                                                                    | Year | Category                                       |Paper Link                                                                                           |
|----|--------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|------|------------------------------------------------|------------------------------------------------------------------------------------------------|
| 1 | Subgraph Retrieval Enhanced Model for Multi-hop Knowledge Base Question Answerings   | ACL | 2022 |  Offline KG Guidelines    | [Link](https://aclanthology.org/2022.acl-long.396/)
| 2 | keqing: knowledge-based question answering is a nature chain-of-thought mentor of LLM   | arXiv  | 2023 |  Offline KG Guidelines    | [Link](https://arxiv.org/abs/2401.00426)
| 3 | Explore then Determine: A GNN-LLM Synergy Framework for Reasoning over Knowledge Graph   | arXiv  | 2024 |  Offline KG Guidelines    | [Link](https://arxiv.org/abs/2406.01145) 
| 4 | Graph-constrained Reasoning: Faithful Reasoning on Knowledge Graphs with Large Language Models   | arXiv  | 2024 |  Offline KG Guidelines    | [Link](https://arxiv.org/abs/2410.13080)
| 5 | Reasoning with Trees: Faithful Question Answering over Knowledge Graph   | COLING  | 2025 |  Offline KG Guidelines    | [Link](https://aclanthology.org/2025.coling-main.211/)
| 6 | Empowering Language Models with Knowledge Graph Reasoning for Open-Domain Question Answering   | EMNLP | 2022 |  Online KG Guildlines    | [Link](https://aclanthology.org/2022.emnlp-main.650/)
| 7 | Knowledge-Enhanced Iterative Instruction Generation and Reasoning for Knowledge Base Question Answering   | NLPCC  | 2022 |  Online KG Guildlines    | [Link](https://link.springer.com/chapter/10.1007/978-3-031-17120-8_34)
| 8 | Evaluating and Enhancing Large Language Models for Conversational Reasoning on Knowledge Graphs   | arXiv  | 2023 |  Online KG Guildlines    | [Link](https://arxiv.org/abs/2312.11282)
| 9 | Think-on-Graph: Deep and Responsible Reasoning of Large Language Model on Knowledge Graph   | ICLR   | 2024 |  Online KG Guildlines    | [Link](https://openreview.net/forum?id=nnVO1PvbTv)
| 10 | Think-on-Graph 2.0: Deep and Faithful Large Language Model Reasoning with Knowledge-guided Retrieval Augmented Generation   | ICLR  | 2024 |  Online KG Guildlines    | [Link](https://openreview.net/forum?id=oFBu7qaZpS)
| 11 | KARPA: A Training-free Method of Adapting Knowledge Graph as References for Large Language Model's Reasoning Path Aggregation   | arXiv  | 2024 |  Online KG Guildlines    | [Link](https://arxiv.org/abs/2412.20995)
| 12 | Retrieval and Reasoning on KGs: Integrate Knowledge Graphs into Large Language Models for Complex Question Answering   | EMNLP  | 2024 |  Online KG Guildlines    | [Link](https://aclanthology.org/2024.findings-emnlp.446)
| 13 | HippoRAG: Neurobiologically Inspired Long-Term Memory for Large Language Models   | NeurIPS  | 2024 |  Online KG Guildlines    | [Link](https://proceedings.neurips.cc/paper_files/paper/2024/file/6ddc001d07ca4f319af96a3024f6dbd1-Paper-Conference.pdf)
| 14 | KG-Agent: An Efficient Autonomous Agent Framework for Complex Reasoning over Knowledge Grap   | arXiv  | 2024 |  Agent-based KG Guildlines    | [Link](https://arxiv.org/abs/2402.11163) 
| 15 | ODA: Observation-Driven Agent for integrating LLMs and Knowledge Graphs   | ACL Findings  | 2024 |  Agent-based KG Guildlines    | [Link](https://aclanthology.org/2024.findings-acl.442/)     
| 16 | Plan-on-graph: self-correcting adaptive planning of large language model on knowledge graphs   | NeruIPS  | 2024 |  Agent-based KG Guildlines    | [Link](https://openreview.net/pdf?id=CwCUEr6wO5)  
| 17 | AtomR: Atomic Operator-Empowered Large Language Models for Heterogeneous Knowledge Reasoning   | KDD  | 2025 |  Agent-based KG Guildlines    | [Link](https://doi.org/10.1145/3711896.37368)    
| 18 | Youtu-GraphRAG: Vertically Unified Agents for Graph Retrieval-Augmented Complex Reasoning   | arXiv  | 2025 |  Agent-based KG Guildlines    | [Link](https://arxiv.org/abs/2508.19855)    
| 19 | A Collaborative Reasoning Framework Powered by Reinforcement Learning and Large Language Models for Complex Questions Answering over Knowledge Graph | COLING| 2025 |  Collaborative Reasoning   | [Link](https://aclanthology.org/2025.coling-main.712/)  
| 20 | Rule-KBQA: Rule-Guided Reasoning for Complex Knowledge Base Question Answering with Large Language Models | COLING| 2025 |  Rule-Guided Reasoning   | [Link](https://aclanthology.org/2025.coling-main.562/)  

### KGs as Refiner and Filter

| NO | Title                                                                                                        | Venue                                                                                                                                                    | Year | Category                                       |Paper Link                                                                                           |
|----|--------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|------|------------------------------------------------|------------------------------------------------------------------------------------------------|
| 1 | Answer Candidate Type Selection: Text-To-Text Language Model for Closed Book Question Answering Meets Knowledge Graphs   | KONVENS    | 2023 |  KG-Driven Filtering and Validation    | [Link](https://aclanthology.org/2023.konvens-main.16/)
| 2 | KG-Rank: Enhancing Large Language Models for Medical QA with Knowledge Graphs and Ranking Techniques      | BioNLP Workshop           
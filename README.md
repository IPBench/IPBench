# IPBench
[**🌐 Homepage**](https://IPBench.github.io/) | [**🤗 Dataset**](https://huggingface.co/datasets/IPBench/IPBench) | [**🤗 Paper**](https://huggingface.co/papers/2504.15524) | [**📖 arXiv**](https://arxiv.org/abs/2504.15524) | [**GitHub**](https://github.com/IPBench/IPBench)


This repo contains the evaluation code for the paper "[IPBench: Benchmarking the knowledge of Large Language Models in Intellectual Property](https://arxiv.org/abs/2504.15524)"
## 🔔News

- 🥳 [2026-04-06] IPBench was accepted by ACL.
- 🎉 [2025-09-29] We have updated the new version of IPBench on arXiv. ([IPBench: Benchmarking the Knowledge of Large Language Models in Intellectual Property](https://arxiv.org/abs/2504.15524/v2))
- 🧐 [2025-05-07] We have added the results of Qwen3-8B, which require a newer version of vLLM (v0.8.5 or later).
- 🎉 [2025-04-23] Our IPBench paper ([IPBench: Benchmarking the Knowledge of Large Language Models in Intellectual Property](https://arxiv.org/abs/2504.15524)) can be accessed in arXiv!
- 🔥 [2025-04-22] We release the codebase of IPBench.

## Introduction

Intellectual property, especially patents, shares similarities with academic papers in that it encapsulates the essence of domain knowledge across various technical fields. However, it is also governed by the intellectual property legal frameworks of different countries and regions. As such, it carries technical, legal, and economic significance, and is closely connected to real-world intellectual property services. In particular, intellectual property data is a rich, multi-modal data type with immense potential for content mining and analysis. Focusing on the field of intellectual property, we propose a comprehensive four-level IP task taxonomy based on the DOK model. Building on this taxonomy, we developed IPBench, a large language model benchmark consisting of 10,374 data instances across 20 tasks and covering 8 types of IP mechanisms. Compared to existing related benchmarks, IPBench features the largest data scale and the most comprehensive task coverage, spanning technical and legal tasks as well as understanding, reasoning, classification, and generation tasks.

<p align="center">
  <img src="framework.bmp" alt="introduction">
</p>

## Dataset Creation

To bridge the gap between real-world demands and the application of LLMs in the IP field, we introduce the first comprehensive IP task taxonomy. Our taxonomy is based on Webb's Depth of Knowledge (DOK) Theory and is extended to include four hierarchical levels: Information Processing, Logical Reasoning, Discriminant Evaluation, and Creative Generation. It includes an evaluation of models' intrinsic knowledge of IP, along with a detailed analysis of IP text from both point-wise and pairwise perspectives, covering technical and legal aspects.

Building on this taxonomy, we develop **IPBench**, the first comprehensive Intellectual Property Benchmark for LLMs, consisting of 10,374 data points across 20 tasks aimed at evaluating the knowledge and capabilities of LLMs in real-world IP applications.

This holistic evaluation enables us to gain a hierarchical deep insight into LLMs, assessing their capabilities in in-domain memory, understanding, reasoning, discrimination, and creation across different IP mechanisms. Due to the legal nature of the IP field, there are regional differences between countries. Our IPBench is constrained within the legal frameworks of the United States and mainland China, making it a bilingual benchmark.

For more detailed information, please refer to our paper and Hugging Face datasets:

- [**📖 arXiv**](https://arxiv.org/abs/2504.15524)
- [**🤗 Dataset**](https://huggingface.co/datasets/IPBench/IPBench)


## Installation
```python
pip install -r requirements.txt
```

## Inference

We provide the inference code using either vLLM or the OpenAI API in the *src* folder, along with corresponding run scripts in the *scripts* folder.
```
sh inference.sh

sh inference-api.sh

sh inference-fewshot.sh

sh inference-cot.sh
```

## Evaluation

We provide separate evaluation code for MCQA, Classification, and Generation tasks in the *eval* folder, along with corresponding run scripts in the *scripts* folder.
```
sh eval-mcqa.sh

sh eval-3-5.sh

sh eval-classification.sh

sh eval-generation.sh
```

## Disclaimers
In developing IPBench, all data are collected exclusively from open and publicly available sources. We strictly adhered to all relevant copyright and licensing regulations. Any data originating from websites or platforms that prohibit copying, redistribution, or automated crawling are explicitly excluded from use. Furthermore, we confirm that all data are used solely for academic and research purposes, and not for any commercial applications. We are committed to upholding responsible data usage and transparency in our research practices. Future updates of IPBench will continue to follow the same principles and remain fully open to academic scrutiny and community feedback.

## Contact
Qiyao Wang: wangqiyao25@mails.ucas.ac.cn

Shiwen Ni: sw.ni@siat.ac.cn

If you have any questions, please feel free to contact us.

## Citation

**BibTeX:**
```bibtex
@article{wang2025ipbench,
  title={IPBench: Benchmarking the Knowledge of Large Language Models in Intellectual Property},
  author={Wang, Qiyao and Chen, Guhong and Wang, Hongbo and Liu, Huaren and Zhu, Minghui and Qin, Zhifei and Li, Linwei and Yue, Yilin and Wang, Shiqiang and Li, Jiayan and others},
  journal={arXiv preprint arXiv:2504.15524},
  year={2025}
}
```

## Star History
[![Star History Chart](https://api.star-history.com/svg?repos=IPBench/IPBench&type=Date)](https://star-history.com/#IPBench/IPBench&Date)

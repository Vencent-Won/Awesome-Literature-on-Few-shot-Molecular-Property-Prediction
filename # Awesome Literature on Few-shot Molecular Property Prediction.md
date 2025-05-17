# Awesome Literature on Few-shot Molecular Property Prediction

This repository showcases a curated collection of research literature on few-shot molecular property prediction. We have categorized this literature according to the taxonomies of **Problems** and **Techniques** detailed in our survey paper, titled Few-shot Molecular Property Prediction: A Survey. In this repository, we primarily arrange the literature based on our  **taxonomy** for clarity. For a deeper understanding of this rapidly evolving and challenging field, we encourage readers to consult our survey.

For our taxonomy, we ategorize existing approaches into three main groups, data, model, and learning paradigm, based on how prior knowledge is utilized. According to the differences in molecular mining strategies, stages of representation learning, and generalization-oriented optimization mechanisms, We further distill this into a more fine-grained classification, to capture the methodological landscape better.



## Our Survey Paper



## Overview

The outline corresponds to the taxonomy in our survey paper.

- [1. Data-level](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#1-Data-Level)
  - [1.1 Generating Samples from Molecules](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#11-Generating-Samples-from-Molecules)
  - [1.2 Modeling Implicit Relations of Molecules](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#12-Modeling-Implicit-Relations-of-Molecules)
  - [1.3 Hybird Methods](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#13-Hybird-Methods)
- [2. Model-level](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#2-Model-level)
  - [2.1 Molecular Intrinsic Representation Learning](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#21-Molecular-Intrinsic-Representation-Learning)
  - [2.2 Molecular Context-Aware Learning](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#22-Molecular-Context-Aware-Learning)
- [3. Learning Paradigm](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#3-Learning-Paradigm)
  - [3.1 Adapter-based Intrinsic Generalization Mechanisms](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#31-Adapter-based-Intrinsic-Generalization-Mechanisms)
  - [3.2 Algorithm Redefinition-Based Parameter Optimization Strategies](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#32-Algorithm-Redefinition-Based-Parameter-Optimization-Strategies)
  - [3.3 Other Strategies](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#33-Other-Strategies)



## Literature

### 1. Data-Level

#### 1.1 Generating Samples from Molecules

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
|Meta-MGNN| Few-shot graph learning for molecular property prediction | WWW 2021 | [PDF](https://arxiv.org/abs/2102.07916) | [Torch](https://github.com/zhichunguo/Meta-MGNN) |
| MTA | Meta-learning with motif-based task augmentation for few-shot molecular property prediction | SDM 2023 | [PDF](https://epubs.siam.org/doi/pdf/10.1137/1.9781611977653.ch91) | [N/A] |
| Molfescue | Molfescue: enhancing molecular property prediction in data-limited and imbalanced contexts using few-shot and contrastive learning | NeurIPS 2021 | [PDF](https://papers.nips.cc/paper/2021/file/91bc333f6967019ac47b49ca0f2fa757-Paper.pdf) | [Torch](https://github.com/tata1661/PAR-NeurIPS21) |


#### 1.1.2 Modeling Implicit Relations of Molecules 

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
| PAR | Property-aware relation networks for few-shot molecular property prediction | ECML PKDD 2016 | [PDF](https://link.springer.com/chapter/10.1007/978-3-319-46227-1_11) |[N/A]|
|Meta-Link| RELATIONAL MULTI-TASK LEARNING: MODELING RELATIONS BETWEEN DATA AND TASKS | ICLR 2022 | [PDF](https://openreview.net/pdf?id=8Py-W8lSUgy) | [Torch](https://github.com/snap-stanford/GraphGym) |
| HSL-RG | Few-shot molecular property prediction via hierar- chically structured learning on relation graphs | Neural Networks 2021 | [PDF](https://www.sciencedirect.com/science/article/pii/S0893608023001685) |  [N/A] |
|GS-Meta| Graph sampling-based meta-learning for molecular property prediction | IJCAI 2023 | [PDF](https://www.ijcai.org/proceedings/2023/0526.pdf) | [Torch](https://github.com/HICAI-ZJU/GS-Meta) |
|KRGTS| Knowledge-enhanced relation graph and task sam- pling for few-shot molecular property prediction | Information Sciences 2025 | [PDF](https://arxiv.org/pdf/2405.15544) | [Torch](https://github.com/Vencent-Won/KRGTS-public) |


#### 1.1.3 Hybird Methods

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
| IGNTE | Implicit geometry and interaction embeddings improve few- shot molecular property prediction | NeurIPS MLSBW 2023 | [PDF](https://www.mlsb.io/papers_2023/Implicit_Geometry_and_Interaction_Embeddings_Improve_Few-Shot_Molecular_Property_Prediction.pdf) | [Torch](https://github.com/cfifty/IGNITE) |
|PG-DERN| Property-guided few-shot learning for molecular property prediction with dual-view encoder and relation graph learning network | IEEE JBHI 2024 | [PDF](https://arxiv.org/abs/2102.07916) | [Torch](https://github.com/Bombtsti/PG-DERN) |


### 2. Model-Level

#### 2.1 Molecular Intrinsic Representation Learning

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
|SMF-GIN| Structure-enhanced meta-learning for few-shot graph classification | AI Open 2021 | [PDF](https://doi.org/10.1016/j.aiopen.2021.08.001) | [Torch](https://github.com/jiangshunyu/SMF-GIN) |
|Meta-GAT| Few-shot graph learning for molecular property prediction | WWW 2021 | [PDF](https://ieeexplore.ieee.org/document/10059171) | [Torch](https://github.com/lol88/Meta-GAT) |
|PH-Mol| Prompting meta-learned hierarchical graph network for molecular property prediction | MedAI 2023 | [PDF](https://ieeexplore.ieee.org/abstract/document/10403216) | [Torch](https://github.com/HICAI-ZJU/PH-Mol) |
|AttFPGNN-MAML| Meta learning with attention based fp-gnns for few-shot molecular property prediction | ACS Omega 2024 | [PDF](https://pubs.acs.org/doi/pdf/10.1021/acsomega.4c02147) | [Torch](https://github.com/sanomics-lab/AttFPGNN-MAML) |


#### 2.2 Molecular Context-Aware Learning

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
|IterRefLSTM| Low data drug discovery with one-shot learning | WWW 2021 | [PDF](https://pubs.acs.org/doi/pdf/10.1021/acscentsci.6b00367) | [Tensorflow](https://github.com/deepchem/deepchem) |
|CAMP| In-context learning for few-shot molecular property prediction | arXiv 2023 | [PDF](https://arxiv.org/pdf/2310.08863) | [N/A] |
|FS-GNNcvTR| Convolutional Transformer via Graph Embeddings for Few-shot Toxicity and Side Effect Prediction | ESANN 2023 | [PDF](https://www.esann.org/sites/default/files/proceedings/2023/ES2023-66.pdf) | [N/A] |
|FS-GNNTR| Few-shot learning with transformers via graph embeddings for molecular property prediction | ESWA 2023 | [PDF](https://www.sciencedirect.com/science/article/pii/S0957417423005079) | [Torch](https://github.com/ltorres97/FS-GNNTR) |
|MHNfs| CONTEXT-ENRICHED MOLECULE REPRESENTATIONS IMPROVE FEW-SHOT DRUG DISCOVERY | ICLR 2023 | [PDF](https://openreview.net/pdf?id=XrMWUuEevr) | [Torch](https://github.com/ml-jku/MHNfs) |
|FS-CrossTR| Multi-scale cross-attention transformer via graph embeddings for few-shot molecular property prediction | ASoC 2024 | [PDF](https://doi.org/10.1016/j.asoc.2024.111268) | [Torch](https://github.com/ltorres97/FS-CrossTR) |
|ICLPP| In-Context Learning of Physical Properties: Few-Shot Adaptation to Out-of-Distribution Molecular Graphs | arXiv 2024 | [PDF](https://arxiv.org/pdf/2406.01808) | [Torch](https://github.com/zhichunguo/Meta-MGNN) |
|CRA| Contextual Representation Anchor Network for Mitigating Selection Bias in Few-Shot Drug Discovery | arXiv 2024 | [PDF](https://arxiv.org/abs/2102.07916) | [N/A] |


### 3. Learning Paradigm

#### 3.1 Adapter-based Intrinsic Generalization Mechanisms

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
| ATGNN | Adaptive Transfer of Graph Neural Networks for Few-Shot Molecular Property Prediction | IEEE TCBB 2023 | [PDF](https://ieeexplore.ieee.org/document/10296036) | [N/A] |
|EM3P2| Few-shot graph learning for molecular property prediction | Bioinformatics 2023 | [PDF](https://doi.org/10.1093/bioinformatics/btad604) | [Torch](https://github.com/Ajou-DILab/EM3P2) |
|PACIA| PACIA: Parameter-Efficient Adapter for Few-Shot Molecular Property Prediction | IJCAI 2024 | [PDF](https://www.ijcai.org/proceedings/2024/0576.pdf) | [Torch](https://github.com/LARS-research/PACIA) |
|Pin-Tuning| Pin-tuning: Parameter-efficient in-context tuning for few-shot molecular property prediction | NeurIPS 2024 | [PDF](https://proceedings.neurips.cc/paper_files/paper/2024/file/82a9fb94035dad3ec007de4ad13c6748-Paper-Conference.pdf) | [Torch](https://github.com/CRIPAC-DIG/Pin-Tuning) |

#### 3.2 Algorithm Redefinition-Based Parameter Optimization Strategies

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
| ADKF-IFT | Meta-learning adaptive deep kernel gaussian processes for molecular property prediction | ICLR 2023 | [PDF](https://wenlin-chen.github.io/publication/chen2023meta/chen2023meta.pdf) | [Torch](https://github.com/Wenlin-Chen/ADKF-IFT)|
|QUADRATIC-PROBE| A Strong Baseline for Molecular Few-Shot Learning | Transactions on Machine Learning Research 2025 | [PDF](https://openreview.net/pdf?id=JQ0agisXny) | [Torch](https://github.com/Fransou/Strong-Baseline-Molecular-FSL) |

#### 3.3 Other Strategiess

| Name| Title| Venue| Paper | Code |
| --- | -----| -----| ------| -----|
| CPRG | Chemical property relation guided few-shot molecular property prediction | IJCNN 2022 | [PDF](https://ieeexplore.ieee.org/document/9892419) | [N/A] |
|Meta-MolNet| Meta-MolNet: A Cross-Domain Benchmark for Few Examples Drug Discovery | IEEE TNNLS 2024 | [PDF](https://ieeexplore.ieee.org/document/10436119) | [Torch](https://github.com/lvqiujie/Meta-MolNet) |
|  AR-APM | Autoregressive activity prediction for low-data drug discovery | ICLR 2024 PML4LRS | [PDF](https://openreview.net/pdf?id=x8mBneTsyF) | [Torch](https://github.com/ml-jku/autoregressive_activity_prediction)|

## Acknowledgements

This page is contributed and maintained by [name](github_url) (e-mail). If you have any suggestions or questions, please feel free to contact us.
# Awesome Literature on Few-shot Molecular Property Prediction

This repository showcases a curated collection of research literature on few-shot molecular property prediction. We have categorized this literature according to the taxonomies of **Problems** and **Techniques** detailed in our survey paper, titled Few-shot Molecular Property Prediction: A Survey. In this repository, we primarily arrange the literature based on our **taxonomy** for clarity. For a deeper understanding of this rapidly evolving and challenging field, we encourage readers to consult our survey.

For our taxonomy, we categorize existing approaches into three main groups, data, model, and learning paradigm, based on how prior knowledge is utilized. According to the differences in molecular mining strategies, stages of representation learning, and generalization-oriented optimization mechanisms, We further distill this into a more fine-grained classification, to capture the methodological landscape better.



## Our Survey Paper



## Overview

The outline corresponds to the taxonomy in our survey paper.

- [1. Data-level](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#1-Data-Level)
  - [1.1 Generative Molecule Data Augmentation](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#11-Generating-Samples-from-Molecules)
  - [1.2 Implicit Molecule Relation Construction](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#12-Modeling-Implicit-Relations-of-Molecules)
  - [1.3 Hybird Methods](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#13-Hybird-Methods)
- [2. Model-level](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#2-Model-level)
  - [2.1 Molecular Intrinsic Representation Learning](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#21-Molecular-Intrinsic-Representation-Learning)
  - [2.2 Molecular Context-aware Learning](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#22-Molecular-Context-Aware-Learning)
- [3. Learning Paradigm](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#3-Learning-Paradigm)
  - [3.1 Adapter-based Intrinsic Generalization Mechanisms](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#31-Adapter-based-Intrinsic-Generalization-Mechanisms)
  - [3.2 Algorithm Redefinition-based Parameter Optimization Strategies](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#32-Algorithm-Redefinition-Based-Parameter-Optimization-Strategies)
  - [3.3 Other Strategies](https://github.com/Vencent-Won/Awesome-Literature-on-Few-shot-Molecular-Property-Prediction#33-Other-Strategies)

## Datasets

### 📌 Multi-task Datasets

| Dataset   | Raw Value Available | #Compounds | #Tasks | #Train Tasks | #Test Tasks | %Missing Label | %Active | %Inactive |
| --------- | ------------------- | ---------- | ------ | ------------ | ----------- | -------------- | ------- | --------- |
| SIDER     | -                   | 1,427      | 27     | 21           | 6           | 0.00           | 56.76   | 43.24     |
| Tox21     | -                   | 7,831      | 12     | 9            | 3           | 17.05          | 6.24    | 76.71     |
| ToxCast   | -                   | 8,575      | 617    | 451          | 158         | 14.97          | 12.60   | 72.43     |
| MUV       | -                   | 93,127     | 17     | 12           | 5           | 84.21          | 0.31    | 15.76     |
| PCBA      | -                   | 437,929    | 128    | 118          | 10          | 39.92          | 0.84    | 59.84     |
| QM9       | ✓                   | 133,885    | 12     | 9            | 3           | -              | -       | -         |
| FS-Mol    | ✓                   | 233,786    | 5120   | 4938         | 157         | -              | -       | -         |
| ExCAPE-ML | ✓                   | 955,386    | 526    | -            | -           | -              | -       | -         |
| Alchemy   | ✓                   | 202,579    | 12     | -            | -           | -              | -       | -         |

---

### 📌 Single-task Datasets

| Dataset | Raw Value Available | #Compounds | #All Scaffolds | #Train Scaffolds | #Test Scaffolds | %Active | %Inactive |
| ------- | ------------------- | ---------- | -------------- | ---------------- | --------------- | ------- | --------- |
| GSK3    | -                   | 3,197      | 38             | 28               | 10              | 90.15   | 9.85      |
| JNK3    | -                   | 4,873      | 62             | 50               | 12              | 99.73   | 0.27      |
| HIV     | -                   | 6,386      | 68             | 54               | 14              | 96.32   | 3.68      |
| PDBbind | ✓                   | 1,405      | 14             | 8                | 6               | -       | -         |
| LD50    | ✓                   | 2,300      | 13             | 8                | 5               | -       | -         |
| ZINC    | ✓                   | 20,327     | 18             | 10               | 8               | -       | -         |

## Literature

### 1. Data-Level

#### 1.1 Generating Samples from Molecules

| Name      | Title                                                        | Venue               | Paper                                                        | Code                                              |
| --------- | ------------------------------------------------------------ | ------------------- | ------------------------------------------------------------ | ------------------------------------------------- |
| Meta-MGNN | Few-shot graph learning for molecular property prediction    | WWW 2021            | [PDF](https://arxiv.org/abs/2102.07916)                      | [Torch](https://github.com/zhichunguo/Meta-MGNN)  |
| MTA       | Meta-learning with motif-based task augmentation for few-shot molecular property prediction | SDM 2023            | [PDF](https://epubs.siam.org/doi/pdf/10.1137/1.9781611977653.ch91) | [N/A]                                             |
| Molfescue | Molfescue: enhancing molecular property prediction in data-limited and imbalanced contexts using few-shot and contrastive learning | Bioinformatics 2024 | [PDF](https://academic.oup.com/bioinformatics/article/40/4/btae118/7616990) | [Torch](https://github.com/zhangruochi/MolFeSCue) |


#### 1.1.2 Modeling Implicit Relations of Molecules 

| Name      | Title                                                        | Venue                     | Paper                                                        | Code                                                 |
| --------- | ------------------------------------------------------------ | ------------------------- | ------------------------------------------------------------ | ---------------------------------------------------- |
| PAR       | Property-aware relation networks for few-shot molecular property prediction | NeurIPS 2021              | [PDF](https://papers.nips.cc/paper/2021/file/91bc333f6967019ac47b49ca0f2fa757-Paper.pdf) | [Torch](https://github.com/tata1661/PAR-NeurIPS21)   |
| CPRG      | Chemical property relation guided few-shot molecular property prediction | IJCNN 2022                | [PDF](https://ieeexplore.ieee.org/document/9892419)          | [N/A]                                                |
| Meta-Link | RELATIONAL MULTI-TASK LEARNING: MODELING RELATIONS BETWEEN DATA AND TASKS | ICLR 2022                 | [PDF](https://openreview.net/pdf?id=8Py-W8lSUgy)             | [Torch](https://github.com/snap-stanford/GraphGym)   |
| IGNTE     | Implicit geometry and interaction embeddings improve few- shot molecular property prediction | NeurIPS MLSBW 2023        | [PDF](https://www.mlsb.io/papers_2023/Implicit_Geometry_and_Interaction_Embeddings_Improve_Few-Shot_Molecular_Property_Prediction.pdf) | [Torch](https://github.com/cfifty/IGNITE) |
| GS-Meta   | Graph sampling-based meta-learning for molecular property prediction | IJCAI 2023                | [PDF](https://www.ijcai.org/proceedings/2023/0526.pdf) | [Torch](https://github.com/HICAI-ZJU/GS-Meta) |
| KRGTS     | Knowledge-enhanced relation graph and task sam- pling for few-shot molecular property prediction | Information Sciences 2025 | [PDF](https://www.sciencedirect.com/science/article/pii/S002002552500489X) | [Torch](https://github.com/Vencent-Won/KRGTS-public)|
| M-GLC     | M-GLC: Motif-Driven Global-Local Context Graphs for Few-shot Molecular Property Prediction | arXiv 2025 | [PDF](https://arxiv.org/pdf/2510.21088) | [N/A] |
| CaMol     | Context-aware Graph Causality Inference for Few-Shot Molecular Property Prediction | arXiv 2026 | [PDF](https://arxiv.org/pdf/2601.11135) | [N/A] |
| ReCoG     | ReCoG: Relational and Compact Context Graph Learning for Few-shot Molecular Property Prediction | ICML 2026 | [PDF](https://openreview.net/pdf?id=lmhLWnIVOk) | [Torch](https://github.com/Vencent-Won/ReCoG-main) |


#### 1.1.3 Hybird Methods

| Name    | Title                                                        | Venue                | Paper                                                        | Code                                         |
| ------- | ------------------------------------------------------------ | -------------------- | ------------------------------------------------------------ | -------------------------------------------- |
| HSL-RG  | Few-shot molecular property prediction via hierarchically structured learning on relation graphs | Neural Networks 2021 | [PDF](https://www.sciencedirect.com/science/article/pii/S0893608023001685) | [N/A]                                        |
| PG-DERN | Property-guided few-shot learning for molecular property prediction with dual-view encoder and relation graph learning network | IEEE JBHI 2024       | [PDF](https://arxiv.org/abs/2102.07916)                      | [Torch](https://github.com/Bombtsti/PG-DERN) |


### 2. Model-Level

#### 2.1 Molecular Intrinsic Representation Learning

| Name          | Title                                                        | Venue                    | Paper                                                        | Code                                                   |
| ------------- | ------------------------------------------------------------ | ------------------------ | ------------------------------------------------------------ | ------------------------------------------------------ |
| SMF-GIN       | Structure-enhanced meta-learning for few-shot graph classification | AI Open 2021             | [PDF](https://doi.org/10.1016/j.aiopen.2021.08.001)          | [Torch](https://github.com/jiangshunyu/SMF-GIN)        |
| Meta-GAT      | Few-shot graph learning for molecular property prediction    | IEEE TNNLS 2023          | [PDF](https://ieeexplore.ieee.org/document/10059171)         | [Torch](https://github.com/lol88/Meta-GAT)             |
| PH-Mol        | Prompting meta-learned hierarchical graph network for molecular property prediction | MedAI 2023               | [PDF](https://ieeexplore.ieee.org/abstract/document/10403216) | [Torch](https://github.com/HICAI-ZJU/PH-Mol)           |
| FS-GNNcvTR    | Convolutional Transformer via Graph Embeddings for Few-shot Toxicity and Side Effect Prediction | ESANN 2023               | [PDF](https://www.esann.org/sites/default/files/proceedings/2023/ES2023-66.pdf) | [N/A]                                                  |
| FS-GNNTR      | Few-shot learning with transformers via graph embeddings for molecular property prediction | ESWA 2023                | [PDF](https://www.sciencedirect.com/science/article/pii/S0957417423005079) | [Torch](https://github.com/ltorres97/FS-GNNTR)         |
| APN           | Attribute-guided prototype network for few-shot molecular property prediction | BIB 2024                 | [PDF](https://doi.org/10.1093/bib/bbae394)                   | [Torch](https://github.com/hou29/few-shot-MPP)         |
| FS-CrossTR    | Multi-scale cross-attention transformer via graph embeddings for few-shot molecular property prediction | ASoC 2024                | [PDF](https://doi.org/10.1016/j.asoc.2024.111268)            | [Torch](https://github.com/ltorres97/FS-CrossTR)       |
| AttFPGNN-MAML | Meta learning with attention based fp-gnns for few-shot molecular property prediction | ACS Omega 2024           | [PDF](https://pubs.acs.org/doi/pdf/10.1021/acsomega.4c02147) | [Torch](https://github.com/sanomics-lab/AttFPGNN-MAML) |
| FS-GcvTR      | Rethinking transformers with convolution and graph embeddings for few-shot molecular property discovery | Pattern Recognition 2025 | [PDF](https://doi.org/10.1016/j.patcog.2025.111657)          | [Torch]( https://github.com/ltorres97/FSGCvTR)         |
| AdaptMol      | AdaptMol：Adaptive Fusion from Sequence String to Topological Structure for Few-shot Drug Discovery | arXiv 2025               | [PDF](https://arxiv.org/abs/2505.11878) | [N/A] |
| Meta-GraphKAN      | Meta-GraphKAN:Few-Shot Graph Kolmogorov Arnold learning Networks for Molecular Property Prediction | IJCNN 2025               | [PDF](https://ieeexplore.ieee.org/abstract/document/11229267) | [Torch](https://github.com/liuyu-0708/Meta-GraphKAN/) |
| Meta-GTMP      | Advancing mutagenicity predictions in drug discovery with an explainable few-shot deep learning framework | Digital Discovery 2025 | [PDF](https://pubs.rsc.org/en/content/articlelanding/2025/dd/d5dd00276a) | [Torch](https://github.com/ltorres97/Meta-GTMP) |
| MolVision      | MolVision: Molecular Property Prediction with Vision Language Models | NeurIPS 2025 | [PDF](https://neurips.cc/virtual/2025/loc/san-diego/poster/121822) | [Torch](https://github.com/molvision/MolVision) |

#### 2.2 Molecular Context-Aware Learning

| Name         | Title                                                        | Venue                    | Paper                                                        | Code                                               |
| ------------ | ------------------------------------------------------------ | ------------------------ | ------------------------------------------------------------ | -------------------------------------------------- |
| IterRefLSTM  | Low data drug discovery with one-shot learning               | ACS central science 2017 | [PDF](https://pubs.acs.org/doi/pdf/10.1021/acscentsci.6b00367) | [Tensorflow](https://github.com/deepchem/deepchem) |
| CAMP         | In-context learning for few-shot molecular property prediction | arXiv 2023               | [PDF](https://arxiv.org/pdf/2310.08863)                      | [N/A]                                              |
| MHNfs        | CONTEXT-ENRICHED MOLECULE REPRESENTATIONS IMPROVE FEW-SHOT DRUG DISCOVERY | ICLR 2023                | [PDF](https://openreview.net/pdf?id=XrMWUuEevr)              | [Torch](https://github.com/ml-jku/MHNfs)           |
| CRA          | Contextual Representation Anchor Network for Mitigating Selection Bias in Few-Shot Drug Discovery | arXiv 2024               | [PDF](https://arxiv.org/pdf/2410.20711)                      | [N/A]                                              |
| ICLPP        | In-Context Learning of Physical Properties: Few-Shot Adaptation to Out-of-Distribution Molecular Graphs | arXiv 2024               | [PDF](https://arxiv.org/pdf/2406.01808)                      | [N/A]                                              |
| MolecularGPT | MolecularGPT：Open Large Language Model (LLM) for Few-Shot Molecular Property Prediction | arXiv 2024               | [PDF](https://arxiv.org/abs/2406.12950)                      | [Torch](https://github.com/NYUSHCS/MolecularGPT)   |
| UniMatch     | UNIMATCH：UNIVERSAL MATCHING FROM ATOM TO TASK FOR FEW-SHOT DRUG DISCOVERY | ICLR 2025                | [PDF](https://iclr.cc/media/iclr-2025/Slides/27929.pdf)      | [Torch](https://github.com/Lirain21/UniMatch.git)  |


### 3. Learning Paradigm

#### 3.1 Adapter-based Intrinsic Generalization Mechanisms

| Name       | Title                                                        | Venue               | Paper                                                        | Code                                              |
| ---------- | ------------------------------------------------------------ | ------------------- | ------------------------------------------------------------ | ------------------------------------------------- |
| ATGNN      | Adaptive Transfer of Graph Neural Networks for Few-Shot Molecular Property Prediction | IEEE TCBB 2023      | [PDF](https://ieeexplore.ieee.org/document/10296036)         | [N/A]                                             |
| EM3P2      | Few-shot graph learning for molecular property prediction    | Bioinformatics 2023 | [PDF](https://doi.org/10.1093/bioinformatics/btad604)        | [Torch](https://github.com/Ajou-DILab/EM3P2)      |
| PACIA      | PACIA: Parameter-Efficient Adapter for Few-Shot Molecular Property Prediction | IJCAI 2024          | [PDF](https://www.ijcai.org/proceedings/2024/0576.pdf)       | [Torch](https://github.com/LARS-research/PACIA)   |
| Pin-Tuning | Pin-tuning: Parameter-efficient in-context tuning for few-shot molecular property prediction | NeurIPS 2024        | [PDF](https://proceedings.neurips.cc/paper_files/paper/2024/file/82a9fb94035dad3ec007de4ad13c6748-Paper-Conference.pdf) | [Torch](https://github.com/CRIPAC-DIG/Pin-Tuning) |

#### 3.2 Algorithm Redefinition-Based Parameter Optimization Strategies

| Name            | Title                                                        | Venue     | Paper                                                        | Code                                                         |
| --------------- | ------------------------------------------------------------ | --------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ADKF-IFT        | Meta-learning adaptive deep kernel gaussian processes for molecular property prediction | ICLR 2023 | [PDF](https://wenlin-chen.github.io/publication/chen2023meta/chen2023meta.pdf) | [Torch](https://github.com/Wenlin-Chen/ADKF-IFT)             |
| QUADRATIC-PROBE | A Strong Baseline for Molecular Few-Shot Learning            | TMLR 2025 | [PDF](https://openreview.net/pdf?id=JQ0agisXny)              | [Torch](https://github.com/Fransou/Strong-Baseline-Molecular-FSL) |
| Meta-Mol | Pushing the boundaries of few-shot learning for low-data drug discovery with a Bayesian meta-learning hypernetwork framework            | BIB 2025 | [PDF](https://doi.org/10.1093/bib/bbaf408) | [Torch](https://github.com/jiacai0101/Meta-Mol) |

#### 3.3 Other Strategiess

| Name        | Title                                                        | Venue           | Paper                                                | Code                                                         |
| ----------- | ------------------------------------------------------------ | --------------- | ---------------------------------------------------- | ------------------------------------------------------------ |
| Meta-MolNet | Meta-MolNet: A Cross-Domain Benchmark for Few Examples Drug Discovery | IEEE TNNLS 2024 | [PDF](https://ieeexplore.ieee.org/document/10436119) | [Torch](https://github.com/lvqiujie/Meta-MolNet)             |
| AR-APM      | Autoregressive activity prediction for low-data drug discovery | JDMLR 2024      | [PDF](https://openreview.net/pdf?id=x8mBneTsyF)      | [Torch](https://github.com/ml-jku/autoregressive_activity_prediction) |



## Performance

<table style="font-size: 0.6em; text-align: center; padding: 1px 1px 1px 1px; white-space: nowrap;"border-collapse: separate; border-spacing: 3px;>
	<caption>
		The performance of FSMPP methods. Among them, Tox21, SIDER, MUV, and ToxCast are evaluated using ROC-AUC, while FS-Mol adopts &#916;AU-PRC as its evaluation metric.
	</caption>
	<tr>
		<td rowspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;">			Taxonomy		</td>
		<td rowspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;" >			Method		</td>
		<td rowspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;" >			Venue		</td>
		<td rowspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;" >			Year		</td>
		<td colspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;">			Tox21		</td>
		<td colspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;">			SIDER		</td>
		<td colspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;">			MUV		</td>
		<td colspan="2"; style="border-top: 2px solid #000; border-bottom: 1px solid #000;">			ToxCast		</td>
		<td style="border-top: 2px solid #000; border-bottom: 1px solid #000;">			FS-Mol		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px solid #000;">			1-shot		</td>
		<td style="border-bottom: 1px solid #000;">			10-shot		</td>
		<td style="border-bottom: 1px solid #000;">			1-shot		</td>
		<td style="border-bottom: 1px solid #000;">			10-shot		</td>
		<td style="border-bottom: 1px solid #000;">			1-shot		</td>
		<td style="border-bottom: 1px solid #000;">			10-shot		</td>
		<td style="border-bottom: 1px solid #000;">			1-shot		</td>
		<td style="border-bottom: 1px solid #000;">			10-shot		</td>
		<td style="border-bottom: 1px solid #000;">			8-shot		</td>
	</tr>
	<tr>
		<td rowspan="13" style="writing-mode: vertical-lr; transform: rotate(180deg); border-bottom: 1px solid #000;">
			Data-Level		</td>
		<td >			Meta-MGNN;		</td>
		<td >			WWW		</td>
		<td >			2021		</td>
		<td >			82.13 &plusmn; 0.13		</td>
		<td >			82.97 &plusmn; 0.10		</td>
		<td >			73.36 &plusmn; 0.32		</td>
		<td >			75.43 &plusmn; 0.21		</td>
		<td >			64.12 &plusmn; 1.18		</td>
		<td >			66.48 &plusmn; 2.12		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			MTA(Pre-PAR)&nbsp;		</td>
		<td >			SDM		</td>
		<td >			2023		</td>
		<td >			84.15 &plusmn; 0.60		</td>
		<td >			86.69 &plusmn; 0.73		</td>
		<td >			76.53 &plusmn; 0.94		</td>
		<td >			79.73 &plusmn; 0.88		</td>
		<td >			70.75 &plusmn; 1.15		</td>
		<td >			71.49 &plusmn; 1.06		</td>
		<td >			75.29 &plusmn; 0.92		</td>
		<td >			76.27 &plusmn; 1.12		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px solid #000;">			MolFeSCue&nbsp;		</td>
		<td style="border-bottom: 1px solid #000;">			Bioinformatics		</td>
		<td style="border-bottom: 1px solid #000;">			2024		</td>
		<td style="border-bottom: 1px solid #000;">			82.05 &plusmn; 0.11		</td>
		<td style="border-bottom: 1px solid #000;">			85.93 &plusmn; 0.10		</td>
		<td style="border-bottom: 1px solid #000;">			73.13 &plusmn; 0.56		</td>
		<td style="border-bottom: 1px solid #000;">			79.08 &plusmn; 0.14		</td>
		<td style="border-bottom: 1px solid #000;">			67.32 &plusmn; 1.08		</td>
		<td style="border-bottom: 1px solid #000;">			72.96 &plusmn; 1.18		</td>
		<td style="border-bottom: 1px solid #000;">			76.39 &plusmn; 1.52		</td>
		<td style="border-bottom: 1px solid #000;">			74.82 &plusmn; 1.39		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
	</tr>
	<tr>
		<td >			PAR&nbsp;		</td>
		<td >			NeurIPS		</td>
		<td >			2021		</td>
		<td >			83.01 &plusmn; 0.09		</td>
		<td >			84.93 &plusmn; 0.11		</td>
		<td >			74.46 &plusmn; 0.29		</td>
		<td >			78.08 &plusmn; 0.16		</td>
		<td >			66.94 &plusmn; 1.12		</td>
		<td >			69.96 &plusmn; 1.37		</td>
		<td >			73.63 &plusmn; 1.00		</td>
		<td >			75.12 &plusmn; 0.84		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			CPRG&nbsp;		</td>
		<td >			IJCNN		</td>
		<td >			2022		</td>
		<td >			78.27 &plusmn; (-)		</td>
		<td >			-		</td>
		<td >			76.83 &plusmn; (-)		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			IGNTE&nbsp;		</td>
		<td >			NeurIPS-MLSBW		</td>
		<td >			2023		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			15.70 &plusmn; 0.70		</td>
	</tr>
	<tr>
		<td >			GS-Meta&nbsp;		</td>
		<td >			IJCAI		</td>
		<td >			2023		</td>
		<td >			86.46 &plusmn; 0.55		</td>
		<td >			86.91 &plusmn; 0.41		</td>
		<td >			84.45 &plusmn; 0.26		</td>
		<td >			85.08 &plusmn; 0.54		</td>
		<td >			67.15 &plusmn; 2.04		</td>
		<td >			70.18 &plusmn; 1.25		</td>
		<td >			81.57 &plusmn; 0.18		</td>
		<td >			83.81 &plusmn; 0.16		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			KRGTS&nbsp;		</td>
		<td >			Information Sciences		</td>
		<td >			2025		</td>
		<td >			87.54 &plusmn; 0.11		</td>
		<td >			87.62 &plusmn; 0.29		</td>
		<td >			84.61 &plusmn; 0.16		</td>
		<td >			85.09 &plusmn; 0.31		</td>
		<td >			68.69 &plusmn; 0.60		</td>
		<td >			74.47 &plusmn; 0.82		</td>
		<td >			82.39 &plusmn; 0.29		</td>
		<td >			84.02 &plusmn; 0.10		</td>
		<td >			-		</td>
	</tr>
    <tr>
        <td >M-GLC&nbsp;</td>
        <td >arXiv</td>
        <td >2025</td>
        <td >98.39 &plusmn; 0.85</td>
        <td >98.17 &plusmn; 0.66</td>
        <td >98.89 &plusmn; 0.57</td>
        <td >98.37 &plusmn; 0.83</td>
        <td >79.09 &plusmn; 2.97</td>
        <td >79.31 &plusmn; 1.96</td>
        <td >90.35 &plusmn; 1.62</td>
        <td >90.24 &plusmn; 1.51</td>
        <td >-</td>
    </tr>
    <tr>
        <td >CaMol&nbsp;</td>
        <td >arXiv</td>
        <td >2026</td>
        <td >83.67 &plusmn; 0.38</td>
        <td >92.69 &plusmn; 0.49</td>
        <td >83.36 &plusmn; 0.32</td>
        <td >91.89 &plusmn; 0.66</td>
        <td >76.79 &plusmn; 0.42</td>
        <td >84.76 &plusmn; 0.63</td>
        <td >82.65 &plusmn; 0.68</td>
        <td >89.64 &plusmn; 0.25</td>
        <td >-</td>
    </tr>
    <tr>
        <td style="border-bottom: 1px solid #000;">ReCoG&nbsp;</td>
        <td style="border-bottom: 1px solid #000;">ICML</td>
        <td style="border-bottom: 1px solid #000;">2026</td>
        <td style="border-bottom: 1px solid #000;">91.01 &plusmn; 2.03</td>
        <td style="border-bottom: 1px solid #000;">93.52 &plusmn; 1.47</td>
        <td style="border-bottom: 1px solid #000;">90.06 &plusmn; 1.17</td>
        <td style="border-bottom: 1px solid #000;">93.98 &plusmn; 1.53</td>
        <td style="border-bottom: 1px solid #000;">81.96 &plusmn; 0.42</td>
        <td style="border-bottom: 1px solid #000;">95.94 &plusmn; 1.37</td>
        <td style="border-bottom: 1px solid #000;">86.05 &plusmn; 1.74</td>
        <td style="border-bottom: 1px solid #000;">88.85 &plusmn; 1.39</td>
        <td>-</td>
    </tr>
	<tr>
		<td >			HSL-RG&nbsp;		</td>
		<td >			Neural Network		</td>
		<td >			2023		</td>
		<td >			84.09 &plusmn; 0.20		</td>
		<td >			85.56 &plusmn; 0.28		</td>
		<td >			77.53 &plusmn; 0.41		</td>
		<td >			78.99 &plusmn; 0.33		</td>
		<td >			68.76 &plusmn; 1.05		</td>
		<td >			71.26 &plusmn; 1.08		</td>
		<td >			74.40 &plusmn; 0.82		</td>
		<td >			76.00 &plusmn; 0.81		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px solid #000;">			PG-DERN&nbsp;		</td>
		<td style="border-bottom: 1px solid #000;">			IEEE JBHI		</td>
		<td style="border-bottom: 1px solid #000;">			2024		</td>
		<td style="border-bottom: 1px solid #000;">			84.12 &plusmn; 0.08		</td>
		<td style="border-bottom: 1px solid #000;">			85.25 &plusmn; 0.29		</td>
		<td style="border-bottom: 1px solid #000;">			77.69 &plusmn; 0.38		</td>
		<td style="border-bottom: 1px solid #000;">			79.62 &plusmn; 0.32		</td>
		<td style="border-bottom: 1px solid #000;">			69.66 &plusmn; 1.02		</td>
		<td style="border-bottom: 1px solid #000;">			71.65 &plusmn; 0.26		</td>
		<td style="border-bottom: 1px solid #000;">			74.51 &plusmn; 0.17		</td>
		<td style="border-bottom: 1px solid #000;">			75.21 &plusmn; 0.19		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
	</tr>
	<tr>
		<td rowspan="16" style="writing-mode: vertical-lr; transform: rotate(180deg); border-bottom: 1px solid #000;">
			Model-Level		</td>
		<td >			Meta-GAT		</td>
		<td >			TNNLS		</td>
		<td >			2023		</td>
		<td >			-		</td>
		<td >			82.40 &plusmn; 1.00		</td>
		<td >			-		</td>
		<td >			77.73 &plusmn; 0.72		</td>
		<td >			-		</td>
		<td >			65.22 &plusmn; 0.84		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			PH-Mol&nbsp;		</td>
		<td >			MedAI		</td>
		<td >			2023		</td>
		<td >			83.38 &plusmn; 0.31		</td>
		<td >			84.94 &plusmn; 0.19		</td>
		<td >			80.10 &plusmn; 0.12		</td>
		<td >			82.26&plusmn;0.22		</td>
		<td >			69.62 &plusmn; 1.97		</td>
		<td >			74.93 &plusmn; 0.86		</td>
		<td >			74.05 &plusmn; 0.23		</td>
		<td >			77.23 &plusmn; 0.13		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			FS-GNNcvTR&nbsp;		</td>
		<td >			ESANN		</td>
		<td >			2023		</td>
		<td >			-		</td>
		<td >			77.50 &plusmn; 0.30		</td>
		<td >			-		</td>
		<td >			71.70 &plusmn; 0.40		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			FS-GNNTR&nbsp;		</td>
		<td >			ESWA		</td>
		<td >			2023		</td>
		<td >			-		</td>
		<td >			77.45 &plusmn; 0.21		</td>
		<td >			-		</td>
		<td >			72.12 &plusmn; 0.50		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			APN&nbsp;		</td>
		<td >			Briefings in Bioinformatics		</td>
		<td >			2024		</td>
		<td >			-		</td>
		<td >			84.54 &plusmn; 0.36		</td>
		<td >			-		</td>
		<td >			79.02 &plusmn; 0.72		</td>
		<td >			-		</td>
		<td >			70.63 &plusmn; 0.80		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			FS-CrossTR&nbsp;		</td>
		<td >			Applied Soft Computing		</td>
		<td >			2024		</td>
		<td >			-		</td>
		<td >			77.64 &plusmn; 0.28		</td>
		<td >			-		</td>
		<td >			71.71 &plusmn; 0.52		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			ATFPGNN-MAML&nbsp;		</td>
		<td >			ACS OMEGA		</td>
		<td >			2024		</td>
		<td >			-		</td>
		<td >			86.12 &plusmn; 0.26		</td>
		<td >			-		</td>
		<td >			84.68 &plusmn; 0.01		</td>
		<td >			-		</td>
		<td >			80.21 &plusmn; 0.29		</td>
		<td >			-		</td>
		<td >			78.15 &plusmn; 0.06		</td>
		<td >			23.10 &plusmn; 1.00		</td>
	</tr>
	<tr>
		<td >			FS-GcvTR&nbsp;		</td>
		<td >			Pattern Recognition		</td>
		<td >			2025		</td>
		<td >			-		</td>
		<td >			77.50 &plusmn; 0.30		</td>
		<td >			-		</td>
		<td >			71.70 &plusmn; 0.40		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
    <tr >
		<td >			AdaptMol&nbsp;		</td>
		<td >			arXiv		</td>
		<td >			2025		</td>
		<td >			-		</td>
		<td >			84.93 &plusmn; 0.27		</td>
		<td >			-		</td>
		<td >			81.59 &plusmn; 0.33		</td>
		<td >			-		</td>
		<td >			77.16 &plusmn; 0.54		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
    <tr>
        <td style="border-bottom: 1px solid #000;">Meta-GraphKAN&nbsp;</td>
        <td style="border-bottom: 1px solid #000;">IJCNN</td>
        <td style="border-bottom: 1px solid #000;">2025</td>
        <td style="border-bottom: 1px solid #000;">84.36 &plusmn; 0.12</td>
        <td style="border-bottom: 1px solid #000;">87.63 &plusmn; 0.15</td>
        <td style="border-bottom: 1px solid #000;">81.65 &plusmn; 0.37</td>
        <td style="border-bottom: 1px solid #000;">82.59 &plusmn; 0.18</td>
        <td style="border-bottom: 1px solid #000;">70.65 &plusmn; 1.15</td>
        <td style="border-bottom: 1px solid #000;">73.69 &plusmn; 1.21</td>
        <td style="border-bottom: 1px solid #000;">-</td>
        <td style="border-bottom: 1px solid #000;">-</td>
        <td style="border-bottom: 1px solid #000;">-</td>
    </tr>
	<tr>
		<td >			IterRefLSTM&nbsp;		</td>
		<td >			ACS central science		</td>
		<td >			2017		</td>
		<td >			82.70 &plusmn; 0.10		</td>
		<td >			82.30 &plusmn; 0.20		</td>
		<td >			69.70 &plusmn; 0.20		</td>
		<td >			66.90 &plusmn; 0.70		</td>
		<td >			47.90 &plusmn; 0.30		</td>
		<td >			49.90 &plusmn; 0.50		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td >			CAMP&nbsp;		</td>
		<td >			arXiv		</td>
		<td >			2023		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			22.90 &plusmn; 0.90		</td>
	</tr>
	<tr>
		<td >			MHNfs&nbsp;		</td>
		<td >			ICLR		</td>
		<td >			2023		</td>
		<td >			-		</td>
		<td >			80.23 &plusmn; 0.84		</td>
		<td >			-		</td>
		<td >			65.89 &plusmn; 1.17		</td>
		<td >			-		</td>
		<td >			73.81 &plusmn; 2.53		</td>
		<td >			-		</td>
		<td >			74.91 &plusmn; 0.73		</td>
		<td >			24.10 &plusmn; 0.60		</td>
	</tr>
	<tr>
		<td >			CRANet&nbsp;		</td>
		<td >			arXiv		</td>
		<td >			2024		</td>
		<td >			-		</td>
		<td >			86.41 &plusmn; 0.39		</td>
        <td >			-		</td>
		<td >			80.23 &plusmn; 0.75		</td>
		<td >			-		</td>
		<td >			80.43 &plusmn; 0.34		</td>
		<td >			-		</td>
		<td >			79.24 &plusmn; 0.91		</td>
		<td >			24.40 &plusmn; 0.90		</td>
	</tr>
	<tr>
		<td >			MolecularGPT&nbsp;		</td>
		<td >			arXiv		</td>
		<td >			2024		</td>
		<td >			65.73 &plusmn; (-)		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			-		</td>
		<td >			72.04 &plusmn; (-)		</td>
		<td >			-		</td>
		<td >			59.49 &plusmn; (-)		</td>
		<td >			-		</td>
		<td >			-		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px solid #000;">			UniMatch&nbsp;		</td>
		<td style="border-bottom: 1px solid #000;">			ICLR		</td>
		<td style="border-bottom: 1px solid #000;">			2025		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			86.35 &plusmn; 0.13		</td>
        <td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			80.34 &plusmn; 0.45		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			86.35 &plusmn; 0.76		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			81.63 &plusmn; 0.73		</td>
		<td style="border-bottom: 1px solid #000;">			24.50 &plusmn; 1.10		</td>
	</tr>
	<tr>
		<td rowspan="8" style="writing-mode: vertical-rl; transform: rotate(180deg); border-bottom: 2px solid #000;">
			Learning Paradigm		</td>
		<td>			ATGNN&nbsp;		</td>
		<td>			TCBB		</td>
		<td>			2023		</td>
		<td>			84.12 &plusmn; 0.21		</td>
		<td>			86.05 &plusmn; 0.15		</td>
		<td>			75.84 &plusmn; 0.16		</td>
		<td>			79.88 &plusmn; 0.14		</td>
		<td>			68.03 &plusmn; 1.54		</td>
		<td>			71.48 &plusmn; 1.47		</td>
		<td>			74.37 &plusmn; 0.81		</td>
		<td>			76.08 &plusmn; 0.52		</td>
		<td>			-		</td>
	</tr>
	<tr>
		<td>			EM3P2&nbsp;		</td>
		<td>			Bioinformatics		</td>
		<td>			2023		</td>
		<td>			83.30 &plusmn; (-)		</td>
		<td>			83.40 &plusmn; (-)		</td>
		<td>			79.20 &plusmn; (-)		</td>
		<td>			79.40 &plusmn; (-)		</td>
		<td>			63.70 &plusmn; (-)		</td>
		<td>			69.50 &plusmn; (-)		</td>
		<td>			-		</td>
		<td>			-		</td>
		<td>			-		</td>
	</tr>
	<tr>
		<td>			PACIA&nbsp;		</td>
		<td>			IJCAI		</td>
		<td>			2023		</td>
		<td>			84.35 &plusmn; 0.14		</td>
		<td>			86.40 &plusmn; 0.27		</td>
		<td>			80.70 &plusmn; 0.28		</td>
		<td>			83.97 &plusmn; 0.22		</td>
		<td>			69.26 &plusmn; 2.35		</td>
		<td>			73.43 &plusmn; 1.96		</td>
		<td>			75.09 &plusmn; 0.95		</td>
		<td>			76.22 &plusmn; 0.73		</td>
		<td>			23.60 &plusmn; 0.80		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px solid #000;">			Pin-Tuning&nbsp;		</td>
		<td style="border-bottom: 1px solid #000;">			NeurIPS		</td>
		<td style="border-bottom: 1px solid #000;">			2024		</td>		
        <td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			91.56 &plusmn; 2.57		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			93.41 &plusmn; 3.52		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			73.33 &plusmn; 2.00		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">           83.71 &plusmn; 0.93		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
	</tr>
	<tr>
		<td>			ADKF-IFT&nbsp;		</td>
		<td>			ICLR		</td>
		<td>			2023		</td>
		<td>			80.97 &plusmn; 0.48		</td>
		<td>			86.06 &plusmn; 0.35		</td>
		<td>			62.16 &plusmn; 1.03		</td>
		<td>			70.95 &plusmn; 0.60		</td>
		<td>			67.25 &plusmn; 3.87		</td>
		<td>			95.74 &plusmn; 0.37		</td>
        <td>			71.13 &plusmn; 1.15		</td>
		<td>			76.22 &plusmn; 0.13		</td>
		<td>			-		</td>
	</tr>
    <tr>
        <td>Meta-Mol&nbsp;</td>
        <td>Briefings in Bioinformatics</td>
        <td>2025</td>
        <td>85.40 &plusmn; 0.50</td>
        <td>86.21 &plusmn; 0.35</td>
        <td>83.45 &plusmn; 0.90</td>
        <td>85.53 &plusmn; 0.89</td>
        <td>66.56 &plusmn; 0.84</td>
        <td>69.55 &plusmn; 0.26</td>
        <td>82.13 &plusmn; 0.68</td>
        <td>84.48 &plusmn; 0.54</td>
        <td>-</td>
    </tr>
	<tr>
		<td style="border-bottom: 1px solid #000;">			QUADRATIC-PROBE&nbsp;		</td>
		<td style="border-bottom: 1px solid #000;">			TMLR		</td>
		<td style="border-bottom: 1px solid #000;">			2025		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">			-		</td>
		<td style="border-bottom: 1px solid #000;">	22.70 &plusmn; 1.00		</td>
	</tr>
	<tr>
		<td style="border-bottom: 2px solid #000;"> AR-APM&nbsp;	</td>
    <td style="border-bottom: 2px solid #000;">	JDMLR	</td>
		<td style="border-bottom: 2px solid #000;"> 2024 </td>
		<td style="border-bottom: 2px solid #000;"> - </td>
		<td style="border-bottom: 2px solid #000;"> -	</td>
		<td style="border-bottom: 2px solid #000;"> - </td>
		<td style="border-bottom: 2px solid #000;"style="border-bottom: 2px solid #000;"> - </td>
		<td style="border-bottom: 2px solid #000;"> -	</td>
		<td style="border-bottom: 2px solid #000;"> - </td>
		<td style="border-bottom: 2px solid #000;"> - </td>
		<td style="border-bottom: 2px solid #000;"> - </td>
		<td style="border-bottom: 2px solid #000;"> 18.90 &plusmn; 0.60 </td>
	</tr>

</table>



## Acknowledgements

This page is contributed and maintained by [Zeyu Wang](https://github.com/Vencent-Won) (Vencent_Wang@outlook.com) and [Xin Zheng](https://github.com/Amanda-Zheng) (xin.zheng@griffith.edu.au). If you have any suggestions or questions, please feel free to contact us.

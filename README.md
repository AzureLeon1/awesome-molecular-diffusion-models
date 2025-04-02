# Awesome-Molecular-Diffusion-Models

![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg) 

> This is a collection of papers on leveraging **Diffusion Models** in **Molecular Generative Tasks**. It's based on our survey paper: [Diffusion Models for Molecules: A Survey of Methods and Tasks](https://arxiv.org/pdf/2502.09511).

Diffusion models have emerged as a powerful generative framework with significant applications in molecular science. These models are particularly well-suited for a variety of downstream tasks, including *de novo* molecular generation, molecular optimization, conformer generation, and molecular docking. This approach represents a cutting-edge intersection of AI and molecular science, offering innovative solutions to traditional challenges in molecular design and analysis.

To facilitate further understanding and exploration of molecular diffusion models, this repository provides a curated list of research papers. These selected papers highlight the innovative applications of diffusion models in molecular generative tasks.

*This repository is still a work in progress. If you would like to add other awesome papers, please feel free to create a pull request or contact `liang.wang@cripac.ia.ac.cn` .*

- [Awesome-Molecular-Diffusion-Models](#awesome-molecular-diffusion-models)
  - [Surveys](#surveys)
  - [2D Molecular Generation](#2d-molecular-generation)
    - [Continuous Data Space](#continuous-data-space)
    - [Discrete Data Space](#discrete-data-space)
  - [3D Molecular Generation](#3d-molecular-generation)
    - [Unconditional and Property-based Generation (Inverse Design)](#unconditional-and-property-based-generation-inverse-design)
    - [Target-based Generation (Structure-based Drug Design)](#target-based-generation-structure-based-drug-design)
    - [Fragment-based Generation (Fragment-based Drug Design)](#fragment-based-generation-fragment-based-drug-design)
    - [Composition-based Generation](#composition-based-generation)
  - [2D\&3D Molecular Generation](#2d3d-molecular-generation)
  - [Molecular Optimization](#molecular-optimization)
    - [Scaffold Hopping or R-group Design](#scaffold-hopping-or-r-group-design)
    - [Generalized Molecular Optimization](#generalized-molecular-optimization)
  - [Conformer Generation](#conformer-generation)
  - [Molecular Docking](#molecular-docking)
  - [Transition State Generation](#transition-state-generation)
  - [Retrosynthesis Prediction and Planning](#retrosynthesis-prediction-and-planning)
  - [Molecular Representation Learning](#molecular-representation-learning)
  - [Cite Us](#cite-us)


## Surveys

1. [arXiv 2022] MolGenSurvey: A Systematic Survey in Machine Learning Models for Molecule Design [[paper]](https://arxiv.org/pdf/2203.14500)
2. [JCIM 2024] Diffusion Models in De Novo Drug Design [[paper]](https://pubs.acs.org/doi/epdf/10.1021/acs.jcim.4c01107?ref=article_openPDF)
3. [arXiv 2025] Diffusion Models for Molecules: A Survey of Methods and Tasks [[paper]](https://arxiv.org/pdf/2502.09511)



## 2D Molecular Generation

### Continuous Data Space

1. [**GDSS**, *ICML 2022*] Score-based Generative Modeling of Graphs via the System of Stochastic Differential Equations [[paper]](https://arxiv.org/pdf/2202.02514) [[code]](https://github.com/harryjo97/GDSS)
2. [**CDGS**, *AAAI 2023*] Conditional Diffusion Based on Discrete Graph Structures for Molecular Graph Generation [[paper]](https://arxiv.org/pdf/2301.00427) [[code]](https://github.com/GRAPH-0/CDGS)
3. [**MOOD**, *ICML 2023*] Exploring Chemical Space with Score-based Out-of-distribution Generation [[paper]](https://arxiv.org/pdf/2206.07632) [[code]](https://github.com/SeulLee05/MOOD)
4. [**CGD**, *ICML 2024*] Context-Guided Diffusion for Out-of-Distribution Molecular and Protein Design [[paper]](https://arxiv.org/pdf/2407.11942) [[code]](https://github.com/leojklarner/context-guided-diffusion)


### Discrete Data Space

1. [**DiGress**, *ICLR 2023*] DiGress: Discrete Denoising Diffusion for Graph Generation [[paper]](https://arxiv.org/pdf/2209.14734) [[code]](https://github.com/cvignac/DiGress)
2. [**HGLDM**, *CIKM 2024*] Hierarchical Graph Latent Diffusion Model for Conditional Molecule Generation [[paper]](https://dl.acm.org/doi/pdf/10.1145/3627673.3679547) 
3. [**Graph DiT**, *NeurIPS 2024*] Graph Diffusion Transformers for Multi-Conditional Molecular Generation [[paper]](https://arxiv.org/pdf/2401.13858) [[code]](https://github.com/liugangcode/Graph-DiT)



## 3D Molecular Generation

### Unconditional and Property-based Generation (Inverse Design)

1. [**EDM**, *ICML 2022*] Equivariant Diffusion for Molecule Generation in 3D [[paper]](https://arxiv.org/pdf/2203.17003) [[code]](https://github.com/ehoogeboom/e3_diffusion_for_molecules)
2. [**EDM-Bridge**, *NeurIPS 2022*] Diffusion-based Molecule Generation with Informative Prior Bridges [[paper]](https://arxiv.org/pdf/2209.00865)
3. [**EEGSDE**, *ICLR 2023*] Equivariant Energy-Guided SDE for Inverse Molecular Design [[paper]](https://arxiv.org/pdf/2209.15408) [[code]](https://github.com/gracezhao1997/EEGSDE)
4. [**GeoLDM**, *ICML 2023*] Geometric Latent Diffusion Models for 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2305.01140) [[code]](https://github.com/MinkaiXu/GeoLDM)
5. [**MDM**, *AAAI 2023*] MDM: Molecular Diffusion Model for 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2209.05710) [[code]](https://github.com/tencent-ailab/MDM)
6. [**VoxMol**, *NeurIPS 2023*] 3D molecule generation by denoising voxel grids [[paper]](https://arxiv.org/pdf/2306.07473) [[code]](https://github.com/genentech/voxmol)
7. [**DiffMol**, *ICML Worshop 2023*] DiffMol: 3D Structured Molecule Generation with Discrete Denoising Diffusion Probabilistic Models[[paper]](https://openreview.net/pdf?id=x43ZyXJC9q) 
8. [**GaUDI**, *Nature Computational Science 2023*] Guided diffusion for inverse molecular design [[paper]](https://www.nature.com/articles/s43588-023-00532-0) [[code]](https://gitlab.com/porannegroup/gaudi.)
9. [**SiMGen**, *arXiv 2024*] Zero Shot Molecular Generation via Similarity Kernels [[paper]](https://arxiv.org/pdf/2402.08708) [[code]](https://github.com/RokasEl/simgen)
10. [**ControlMol**, *arXiv 2024*] ControlMol: Adding Substructure Control To Molecule Diffusion Models [[paper]](https://arxiv.org/pdf/2405.06659)
11. [**LDM-3DG**, *ICLR 2024*] Latent 3D Graph Diffusion [paper]](https://openreview.net/pdf?id=cXbnGtO0NZ) [[code]](https://github.com/Shen-Lab/LDM-3DG)
12. [**CGD**, *ICML 2024*] Context-Guided Diffusion for Out-of-Distribution Molecular and Protein Design [paper]](https://arxiv.org/pdf/2407.11942) [[code]](https://github.com/leojklarner/context-guided-diffusion)
13. [**END**, *NeurIPS 2024*] Equivariant Neural Diffusion for Molecule Generation [paper]](https://openreview.net/pdf?id=40pE5pFhWl) [[code]](https://github.com/frcnt/equivariant-neural-diffusion)
14. [**GFMDiff**, *AAAI 2024*] Geometric-Facilitated Denoising Diffusion Model for 3D Molecule Generation [paper]](https://arxiv.org/pdf/2401.02683) 
15. [**MuDM**, *ICLR 2024*] Training-free Multi-objective Diffusion Model for 3D Molecule Generation [paper]](https://openreview.net/pdf?id=X41c4uB4k0)
16. [**EQGAT-diff**, *ICLR 2024*] Navigating the Design Space of Equivariant Diffusion-Based Generative Models for De Novo 3D Molecule Generation [paper]](https://arxiv.org/pdf/2309.17296)
17. [**NExT-Mol**, *ICLR 2025*] NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation [paper]](https://arxiv.org/pdf/2502.12638) [[code]](https://github.com/acharkq/NExT-Mol)

### Target-based Generation (Structure-based Drug Design)

1. [**TargetDiff**, *ICLR 2023*] 3D Equivariant Diffusion for Target-Aware Molecule Generation and Affinity Prediction [paper]](https://arxiv.org/pdf/2303.03543) [[code]](https://github.com/guanjq/targetdiff)
2. [**DiffSBDD**, *Nature Computational Science 2024*] Structure-based drug design with equivariant diffusion models [paper]](https://arxiv.org/pdf/2210.13695) [[code]](https://github.com/arneschneuing/DiffSBDD)
3. [**DecompDiff**, *ICML 2023*] DecompDiff: Diffusion Models with Decomposed Priors for Structure-Based Drug Design [paper]](https://arxiv.org/pdf/2403.07902) [[code]](https://github.com/bytedance/DecompDiff)
4. [**SBE-Diff**, *ICML 2024*] Rethinking specificity in SBDD: Leveraging delta score and energy-guided diffusion [paper]](https://arxiv.org/pdf/2403.12987)
5. [**LDM-3DG**, *ICLR 2024*] Latent 3D Graph Diffusion [paper]](https://openreview.net/pdf?id=cXbnGtO0NZ) [[code]](https://github.com/Shen-Lab/LDM-3DG)
6. [**PMDM**, *Nature Communications 2024*] A dual diffusion model enables 3D molecule generation and lead optimization based on target pockets [paper]](https://www.nature.com/articles/s41467-024-46569-1) [[code]](https://github.com/Layne-Huang/PMDM?tab=readme-ov-file#pmdm-a-dual-diffusion-model-enables-3d-binding-bioactive-molecule-generation-and-lead-optimization-given-target-pockets)
7. [**BindDM**, *AAAI 2024*] Binding-Adaptive Diffusion Models for Structure-Based Drug Design [paper]](https://arxiv.org/pdf/2402.18583) [[code]](https://github.com/YangLing0818/BindDM)
8. [**IRDiff**, *ICML 2024*] Interaction-based Retrieval-augmented Diffusion Models for Protein-specific 3D Molecule Generation [paper]](https://openreview.net/pdf?id=eejhD9FCP3) [[code]](https://github.com/YangLing0818/IRDiff)
9. [**AliDiff**, *NeurIPS 2024*] Aligning Target-Aware Molecule Diffusion Models with Exact Energy Optimization [paper]](https://arxiv.org/pdf/2407.01648) [[code]](https://github.com/MinkaiXu/AliDiff)
10. [**IPDiff**, *ICLR 2024*] Protein-Ligand Interaction Prior for Binding-aware 3D Molecule Diffusion Models [paper]](https://openreview.net/pdf?id=qH9nrMNTIW) [[code]](https://github.com/YangLing0818/IPDiff?tab=readme-ov-file)
11. [**EQGAT-diff**, *ICLR 2024*] Navigating the Design Space of Equivariant Diffusion-Based Generative Models for De Novo 3D Molecule Generation [paper]](https://arxiv.org/pdf/2309.17296)

### Fragment-based Generation (Fragment-based Drug Design)

1. [**DiffLinker**, *Nature Machine Intelligence 2024*] Equivariant 3D-conditional diffusion model for molecular linker design [paper]](https://arxiv.org/pdf/2210.05274) [[code]](https://github.com/igashov/DiffLinker)

### Composition-based Generation

1. [**UniMat**, *ICLR 2024*] Scalable Diffusion for Materials Generation [paper]](https://arxiv.org/pdf/2311.09235)



## 2D\&3D Molecular Generation

1. [**MolDiff**, *ICML 2023*] MolDiff: Addressing the Atom-Bond Inconsistency Problem in 3D Molecule Diffusion Generation [paper]](https://arxiv.org/pdf/2305.07508) [[code]](https://github.com/pengxingang/MolDiff)
2. [**MiDi**, *ECML 2023*] MiDi: Mixed Graph and 3D Denoising Diffusion for Molecule Generation [paper]](https://arxiv.org/pdf/2302.09048) [[code]](https://github.com/cvignac/MiDi)
3. [**JODO**, *TNNLS 2024*] Learning Joint 2-D and 3-D Graph Diffusion Models for Complete Molecule Generation [paper]](https://arxiv.org/pdf/2305.12347) [[code]](https://github.com/GRAPH-0/JODO)
4. [**MUDiff**, *LoG 2023*] MUDiff: Unified Diffusion for Complete Molecule Generation [paper]](https://arxiv.org/pdf/2304.14621) [[code]](https://github.com/WillHua127/mudiff)



## Molecular Optimization

### Scaffold Hopping or R-group Design

1. [**DiffHopp**, *arXiv 2023*] DiffHopp: A Graph Diffusion Model for Novel Drug Design via Scaffold Hopping [paper]](https://arxiv.org/pdf/2308.07416) [[code]](https://github.com/jostorge/diffusion-hopping)
2. [**TurboHopp**, *NeurIPS 2023*] TurboHopp: Accelerated Molecule Scaffold Hopping with Consistency Models [paper]](https://arxiv.org/pdf/2410.20660) [[code]](https://github.com/orgw/TurboHopp)
3. [**PMDM**, *Nature Communications 2024*] A dual diffusion model enables 3D molecule generation and lead optimization based on target pockets [paper]](https://www.nature.com/articles/s41467-024-46569-1) [[code]](https://github.com/Layne-Huang/PMDM)
4. [**DecompOpt**, *ICLR 2024*] DecompOpt: Controllable and Decomposed Diffusion Models for Structure-based Molecular Optimization [paper]](https://arxiv.org/pdf/2403.13829) [[code]](https://github.com/bytedance/DecompOpt)

### Generalized Molecular Optimization

1. [**DiffSBDD**, *Nature Computational Science 2024*] Structure-based drug design with equivariant diffusion models [paper]](https://arxiv.org/pdf/2210.13695) [[code]](https://github.com/arneschneuing/DiffSBDD)


## Conformer Generation

1. [**GeoDiff**, *ICLR 2022*] GeoDiff: a Geometric Diffusion Model for Molecular Conformation Generation [paper]](https://arxiv.org/pdf/2203.02923) [[code]](https://github.com/MinkaiXu/GeoDiff)
2. [**Torsional Diffusion**, *NeurIPS 2022*] Torsional Diffusion for Molecular Conformer Generation [paper]](https://arxiv.org/pdf/2206.01729) [[code]](https://github.com/gcorso/torsional-diffusion)
3. [**DiSCO**, *AAAI 2024*] DiSCO: Diffusion Schrödinger Bridge for Molecular Conformer Optimization [paper]](https://ojs.aaai.org/index.php/AAAI/article/view/29238) [[code]](https://github.com/eugenebang/DiSCO_repo)
4. [**NExT-Mol**, *ICLR 2025*] NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation [paper]](https://arxiv.org/pdf/2502.12638) [[code]](https://github.com/acharkq/NExT-Mol)



## Molecular Docking

1. [**DiffDock**, *ICLR 2023*] DiffDock: Diffusion Steps, Twists, and Turns for Molecular Docking [paper]](https://arxiv.org/pdf/2210.01776) [[code]](https://github.com/gcorso/DiffDock)
2. [**DynamicBind**, *Nature Communications 2024*] DynamicBind: predicting ligand-specific protein-ligand complex structure with a deep equivariant generative model [paper]](https://www.nature.com/articles/s41467-024-45461-2) [[code]](https://github.com/luwei0917/DynamicBind)
3. [**Re-Dock**, *ICML 2024*] Re-Dock: Towards Flexible and Realistic Molecular Docking with Diffusion Bridge [paper]](https://arxiv.org/pdf/2402.11459)



## Transition State Generation

1. [**OA-ReactDiff**, *Nature Computational Science 2023*] Accurate Transition State Generation with an Object-Aware Equivariant Elementary Reaction Diffusion Model [paper]](https://arxiv.org/pdf/2304.06174) [[code]](https://github.com/chenruduan/OAReactDiff)



## Retrosynthesis Prediction and Planning

1. [**DiffAlign**, *arXiv 2024*] Alignment is Key for Applying Diffusion Models to Retrosynthesis [paper]](https://arxiv.org/pdf/2405.17656)
1. [**RetroDiff**, *AISTATS 2025*] RetroDiff: Retrosynthesis as Multi-stage Distribution Interpolation [paper]](https://arxiv.org/pdf/2311.14077)
1. [**GDiffRetro**, *AAAI 2025*] GDiffRetro: Retrosynthesis Prediction with Dual Graph Enhanced Molecular Representation and Diffusion Generation [paper]](https://arxiv.org/pdf/2501.08001) [[code]](https://github.com/sunshy-1/GDiffRetro)



## Molecular Representation Learning

1. [**MoleculeSDE**, *ICML 2023*] A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal Pretraining [paper]](https://arxiv.org/pdf/2305.18407) [[code]](https://github.com/chao1224/MoleculeSDE)
2. [**SubGDiff**, *NeurIPS 2024*] SubGDiff: A Subgraph Diffusion Model to Improve Molecular Representation Learning [paper]](https://arxiv.org/pdf/2405.05665) [[code]](https://github.com/IDEA-XL/SubgDiff)
3. [**UniGEM**, *ICLR 2025*] UniGEM: A Unified Approach to Generation and Property Prediction for Molecules [paper]](https://arxiv.org/pdf/2410.10516) [[code]](https://github.com/fengshikun/UniGEM)



## Cite Us

Please feel free to cite this work if you find it helpful!

```
@article{wang2025survey,
  title={Diffusion Models for Molecules: A Survey of Methods and Tasks},
  author={Liang Wang and Chao Song and Zhiyuan Liu and Yu Rong and Qiang Liu and Shu Wu and Liang Wang},
  journal={arXiv},
  volume={abs/2502.09511}
  year={2025}
}
```

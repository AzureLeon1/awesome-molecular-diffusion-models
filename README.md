# Awesome-Molecular-Diffusion-Models

![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg) 

> This is a collection of papers on leveraging **Diffusion Models** in **Molecular Generative Tasks**. It's based on our survey paper: **Diffusion Models for Molecules: A Survey of Methods and Tasks**.

Diffusion models have emerged as a powerful generative framework with significant applications in molecular science. These models are particularly well-suited for a variety of downstream tasks, including *de novo* molecular generation, molecular optimization, conformer generation, and molecular docking. This approach represents a cutting-edge intersection of AI and molecular science, offering innovative solutions to traditional challenges in molecular design and analysis.

To facilitate further understanding and exploration of molecular diffusion models, this repository provides a curated list of research papers. These selected papers highlight the innovative applications of diffusion models in molecular generative tasks.

*This repository is still a work in progress. If you would like to add other awesome papers, please feel free to create a pull request or contact `liang.wang@cripac.ia.ac.cn` .*

### Surveys

1. [arXiv 2025] Diffusion Models for Molecules: A Survey of Methods and Tasks [[paper]](https://arxiv.org/pdf/2502.09511)
2. [arXiv 2022] MolGenSurvey: A Systematic Survey in Machine Learning Models for Molecule Design [[paper]](https://arxiv.org/pdf/2203.14500)



### 2D Molecular Geneartion

**Continuous Data Space**

1. [ICML 2022] Score-based Generative Modeling of Graphs via the System of Stochastic Differential Equations
2. [AAAI 2023] Conditional Diffusion Based on Discrete Graph Structures for Molecular Graph Generation
3. [ICML 2023] Exploring Chemical Space with Score-based Out-of-distribution Generation
4. [ICML 2024] Context-Guided Diffusion for Out-of-Distribution Molecular and Protein Design

**Discrete Data Space**

1. [ICLR 2023] DiGress: Discrete Denoising Diffusion for Graph Generation
2. [CIKM 2024] Hierarchical Graph Latent Diffusion Model for Conditional Molecule Generation
3. [NeurIPS 2024] Graph Diffusion Transformers for Multi-Conditional Molecular Generation



### 3D Molecular Geneartion

**Unconditional and Property-based Generation (Inverse Design)**

1. [ICML 2022] Equivariant Diffusion for Molecule Generation in 3D
1. [NeurIPS 2022] Diffusion-based Molecule Generation with Informative Prior Bridges
1. [ICLR] 2023] Equivariant Energy-Guided SDE for Inverse Molecular Design
1. [ICML 2023] Geometric Latent Diffusion Models for 3D Molecule Generation
1. [AAAI 2023] MDM: Molecular Diffusion Model for 3D Molecule Generation
1. [NeurIPS 2023] 3D molecule generation by denoising voxel grids
1. [ICML Worshop 2023] DiffMol: 3D Structured Molecule Generation with Discrete Denoising Diffusion Probabilistic Models
1. [Nature Computational Science 2023] Guided diffusion for inverse molecular design
1. [arXiv 2024] Zero Shot Molecular Generation via Similarity Kernels
1. [arXiv 2024] ControlMol: Adding Substructure Control To Molecule Diffusion Models
1. [ICLR 2024] Latent 3D Graph Diffusion
1. [ICML 2024] Context-Guided Diffusion for Out-of-Distribution Molecular and Protein Design
1. [NeurIPS 2024] Equivariant Neural Diffusion for Molecule Generation
1. [AAAI 2024] Geometric-Facilitated Denoising Diffusion Model for 3D Molecule Generation
1. [ICLR 2024] Training-free Multi-objective Diffusion Model for 3D Molecule Generation
1. [ICLR 2024] Navigating the Design Space of Equivariant Diffusion-Based Generative Models for De Novo 3D Molecule Generation
1. [ICLR 2025] NEXT-MOL: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation

**Target-based Generation (Structure-based Drug Design)**

1. [ICLR 2023] 3D Equivariant Diffusion for Target-Aware Molecule Generation and Affinity Prediction
2. [Nature Computational Science 2024] Structure-based drug design with equivariant diffusion models
3. [ICML 2023] DecompDiff: Diffusion Models with Decomposed Priors for Structure-Based Drug Design
4. [ICML 2024] Rethinking specificity in SBDD: Leveraging delta score and energy-guided diffusion
5. [ICLR 2024] Latent 3D Graph Diffusion
6. [Nature Communications 2024] A dual diffusion model enables 3D molecule generation and lead optimization based on target pockets
7. [AAAI 2024] Binding-Adaptive Diffusion Models for Structure-Based Drug Design
8. [ICML 2024] Interaction-based Retrieval-augmented Diffusion Models for Protein-specific 3D Molecule Generation
9. [NeurIPS 2024] Aligning Target-Aware Molecule Diffusion Models with Exact Energy Optimization
10. [ICLR 2024] Protein-Ligand Interaction Prior for Binding-aware 3D Molecule Diffusion Models
11. [ICLR 2024] Navigating the Design Space of Equivariant Diffusion-Based Generative Models for De Novo 3D Molecule Generation

**Fragment-based Generation (Fragment-based Drug Design)**

1. [Nature Machine Intelligence 2024] Equivariant 3D-conditional diffusion model for molecular linker design

**Composition-based Generation**

1. [ICLR 2024] Scalable Diffusion for Materials Generation



### 2D\&3D Molecular Geneartion

1. [ICML 2023] MolDiff: Addressing the Atom-Bond Inconsistency Problem in 3D Molecule Diffusion Generation
2. [ECML 2023] MiDi: Mixed Graph and 3D Denoising Diffusion for Molecule Generation
3. [TNNLS 2024] Learning Joint 2-D and 3-D Graph Diffusion Models for Complete Molecule Generation
4. [LoG 2023] MUDiff: Unified Diffusion for Complete Molecule Generation



### Molecular Optimization

**Scaffold Hopping or R-group Design**

1. [arXiv 2023] DiffHopp: A Graph Diffusion Model for Novel Drug Design via Scaffold Hopping
2. [NeurIPS 2023] TurboHopp: Accelerated Molecule Scaffold Hopping with Consistency Models
3. [Nature Communications 2024] A dual diffusion model enables 3D molecule generation and lead optimization based on target pockets
4. [ICLR 2024] DecompOpt: Controllable and Decomposed Diffusion Models for Structure-based Molecular Optimization

**Generalized Molecular Optimization**

1. [Nature Computational Science 2024] Structure-based drug design with equivariant diffusion models



### Conformer Generation

1. [AAAI 2024] DiSCO: Diffusion Schrödinger Bridge for Molecular Conformer Optimization
2. [ICLR 2025] NEXT-MOL: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation



### Molecular Docking

1. [ICLR 2022] GeoDiff: a Geometric Diffusion Model for Molecular Conformation Generation
2. [NeurIPS 2022] Torsional Diffusion for Molecular Conformer Generation
3. [ICLR 2023] DiffDock: Diffusion Steps, Twists, and Turns for Molecular Docking
4. [ICML 2024] Re-Dock: Towards Flexible and Realistic Molecular Docking with Diffusion Bridge



### Transition State Generation

1. [Nature Computational Science 2023] Accurate Transition State Generation with an Object-Aware Equivariant Elementary Reaction Diffusion Model



### Molecular Representation Learning

1. [ICML 2023] A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal Pretraining
2. [NeurIPS 2024] SubGDiff: A Subgraph Diffusion Model to Improve Molecular Representation Learning
3. [ICLR 2025] UniGEM: A Unified Approach to Generation and Property Prediction for Molecules



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
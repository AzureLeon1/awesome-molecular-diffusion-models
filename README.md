# Awesome-Molecular-Diffusion-Models

![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg) 

> A curated collection of papers on **Diffusion Models** for **Molecular Science**, accompanying our survey: [Diffusion Models for Molecules: A Survey of Methods and Tasks](https://arxiv.org/pdf/2502.09511).

Diffusion models have emerged as a versatile and principled generative framework with broad applications across molecular science. They are particularly well-suited for downstream tasks including *de novo* molecular design, molecular docking, molecular optimization, conformer generation, and molecular structure elucidation, spanning the frontier of AI and molecular science.

This repository curates key research papers advancing the exploration and application of diffusion models to molecular science tasks. Papers are organized by task, with the goal of offering a structured entry point for researchers new to the field and a reference for those tracking the latest developments. 

Contributions are welcome. If you find missing papers or have suggestions for improvement, feel free to open a pull request or reach out at `wangliang.leon20@gmail.com`.

- [Awesome-Molecular-Diffusion-Models](#awesome-molecular-diffusion-models)
  - [Task Taxonomy](#task-taxonomy)
  - [Surveys](#surveys)
  - [Unconditional \& Property-based Generation](#unconditional--property-based-generation)
    - [2D Molecular Generation](#2d-molecular-generation)
    - [3D Molecular Generation](#3d-molecular-generation)
    - [2D\&3D Molecular Generation](#2d3d-molecular-generation)
  - [Structure-based Drug Design](#structure-based-drug-design)
  - [Molecular Docking](#molecular-docking)
  - [Molecular Optimization](#molecular-optimization)
  - [Conformer Generation](#conformer-generation)
  - [Linker Design](#linker-design)
  - [Molecular Structure Elucidation](#molecular-structure-elucidation)
  - [Transition State Generation](#transition-state-generation)
  - [Retrosynthesis Prediction and Planning](#retrosynthesis-prediction-and-planning)
  - [Molecular Representation Learning](#molecular-representation-learning)
  - [Cite Us](#cite-us)


## Task Taxonomy

| Task | Input | Output |
|---|---|---|
| **Unconditional & Property-based Generation** | None / property | Novel molecules |
| **Structure-based Drug Design** | Protein pocket | Ligand |
| **Molecular Docking** | Molecule + protein | Binding pose |
| **Molecular Optimization** | Existing molecule | Improved molecule |
| **Conformer Generation** | 2D molecular graph | 3D conformation |
| **Linker Design** | Molecular fragments | Linker + complete molecule |
| **Molecular Structure Elucidation** | Molecular spectra | Molecular structure |
| **Transition State Generation** | Reactants + products | Transition state structure |
| **Retrosynthesis** | Target molecule | Synthesis pathway |
| **Representation Learning** | Molecule | Latent representation |

## Surveys

1. [arXiv 2022] MolGenSurvey: A Systematic Survey in Machine Learning Models for Molecule Design [[paper]](https://arxiv.org/pdf/2203.14500)
2. [JCIM 2024] Diffusion Models in De Novo Drug Design [[paper]](https://pubs.acs.org/doi/epdf/10.1021/acs.jcim.4c01107?ref=article_openPDF)
3. [arXiv 2025] Diffusion Models for Molecules: A Survey of Methods and Tasks [[paper]](https://arxiv.org/pdf/2502.09511)

## Unconditional & Property-based Generation

### 2D Molecular Generation

**Continuous Data Space**

1. [**GDSS**, *ICML 2022*] Score-based Generative Modeling of Graphs via the System of Stochastic Differential Equations [[paper]](https://arxiv.org/pdf/2202.02514) [[code]](https://github.com/harryjo97/GDSS)
2. [**CDGS**, *AAAI 2023*] Conditional Diffusion Based on Discrete Graph Structures for Molecular Graph Generation [[paper]](https://arxiv.org/pdf/2301.00427) [[code]](https://github.com/GRAPH-0/CDGS)
3. [**MOOD**, *ICML 2023*] Exploring Chemical Space with Score-based Out-of-distribution Generation [[paper]](https://arxiv.org/pdf/2206.07632) [[code]](https://github.com/SeulLee05/MOOD)
4. [**CGD**, *ICML 2024*] Context-Guided Diffusion for Out-of-Distribution Molecular and Protein Design [[paper]](https://arxiv.org/pdf/2407.11942) [[code]](https://github.com/leojklarner/context-guided-diffusion)
5. [**GruM**, *ICML 2024*] Graph Generation with Diffusion Mixture [[paper]](https://arxiv.org/pdf/2302.03596) [[code]](https://github.com/harryjo97/GruM)
6. [**VIDD**, *ICLR 2026*] Iterative Distillation for Reward-Guided Fine-Tuning of Diffusion Models in Biomolecular Design [[paper]](https://openreview.net/pdf?id=NFffW9tBmC) [[code]](https://divelab.github.io/VIDD/)


**Discrete Data Space**

1. [**DiGress**, *ICLR 2023*] DiGress: Discrete Denoising Diffusion for Graph Generation [[paper]](https://arxiv.org/pdf/2209.14734) [[code]](https://github.com/cvignac/DiGress)
2. [**HGLDM**, *CIKM 2024*] Hierarchical Graph Latent Diffusion Model for Conditional Molecule Generation [[paper]](https://dl.acm.org/doi/pdf/10.1145/3627673.3679547) 
3. [**Graph DiT**, *NeurIPS 2024*] Graph Diffusion Transformers for Multi-Conditional Molecular Generation [[paper]](https://arxiv.org/pdf/2401.13858) [[code]](https://github.com/liugangcode/Graph-DiT)
4. [**GBD**, *ICLR 2025*] Advancing Graph Generation through Beta Diffusion [[paper]](https://openreview.net/pdf?id=x1An5a3U9I) [[code]](https://github.com/xinyangATK/GraphBetaDiffusion)
5. [**EDM-SyCo**, *ICLR 2025*] Lift Your Molecules: Molecular Graph Generation in Latent Euclidean Space [[paper]](https://openreview.net/pdf?id=uNomADvF3s) [[code]](https://github.com/ketatam/SyCo)
6. [**GenMol**, *ICML 2025*] GenMol: A Drug Discovery Generalist with Discrete Diffusion [[paper]](https://openreview.net/pdf?id=KM7pXWG1xj) [[code]](https://github.com/NVIDIA-Digital-Bio/genmol)
7. [**DMol**, *NeurIPS 2025*] DMol: A Highly Efficient and Chemical Motif-Preserving Molecule Generation Platform [[paper]](https://openreview.net/pdf?id=5szmKUMhB7) [[code]](https://github.com/liekon/Discrete-Graph-Generation)
8. [**DemoDiff**, *ICLR 2026*] Graph Diffusion Transformers are In-Context Molecular Designers [[paper]](https://openreview.net/pdf?id=lJ87GN5zJc)
9. [**MELD**, *ICLR 2026*] Learning Flexible Forward Trajectories for Masked Molecular Diffusion [[paper]](https://openreview.net/pdf?id=raVuVPbnQL) [[code]](https://holymollyhao.github.io/MELD)
10. [**FragFM**, *ICLR 2026*] FragFM: Hierarchical Framework for Efficient Molecule Generation via Fragment-Level Discrete Flow Matching [[paper]](https://openreview.net/pdf?id=tr6vRn2aPg) [[code]](https://github.com/lee-jwon/FragFM)

### 3D Molecular Generation

1. [**EDM**, *ICML 2022*] Equivariant Diffusion for Molecule Generation in 3D [[paper]](https://arxiv.org/pdf/2203.17003) [[code]](https://github.com/ehoogeboom/e3_diffusion_for_molecules)
2. [**EDM-Bridge**, *NeurIPS 2022*] Diffusion-based Molecule Generation with Informative Prior Bridges [[paper]](https://arxiv.org/pdf/2209.00865)
3. [**EEGSDE**, *ICLR 2023*] Equivariant Energy-Guided SDE for Inverse Molecular Design [[paper]](https://arxiv.org/pdf/2209.15408) [[code]](https://github.com/gracezhao1997/EEGSDE)
4. [**GeoLDM**, *ICML 2023*] Geometric Latent Diffusion Models for 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2305.01140) [[code]](https://github.com/MinkaiXu/GeoLDM)
5. [**HierDiff**, *ICML 2023*] Coarse-to-Fine: a Hierarchical Diffusion Model for Molecule Generation in 3D [[paper]](https://openreview.net/pdf?id=7haEvhb25X) [[code]](https://github.com/qiangbo1222/HierDiff)
6. [**MDM**, *AAAI 2023*] MDM: Molecular Diffusion Model for 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2209.05710) [[code]](https://github.com/tencent-ailab/MDM)
7. [**VoxMol**, *NeurIPS 2023*] 3D molecule generation by denoising voxel grids [[paper]](https://arxiv.org/pdf/2306.07473) [[code]](https://github.com/genentech/voxmol)
8. [**EquiFM**, *NeurIPS 2023*] Equivariant Flow Matching with Hybrid Probability Transport for 3D Molecule Generation [[paper]](https://openreview.net/pdf?id=hHUZ5V9XFu) [[code]](https://github.com/AlgoMole/MolFM)
9. [**DiffMol**, *ICML Worshop 2023*] DiffMol: 3D Structured Molecule Generation with Discrete Denoising Diffusion Probabilistic Models[[paper]](https://openreview.net/pdf?id=x43ZyXJC9q) 
10. [**GaUDI**, *Nature Computational Science 2023*] Guided diffusion for inverse molecular design [[paper]](https://www.nature.com/articles/s43588-023-00532-0) [[code]](https://gitlab.com/porannegroup/gaudi.)
11. [**SiMGen**, *arXiv 2024*] Zero Shot Molecular Generation via Similarity Kernels [[paper]](https://arxiv.org/pdf/2402.08708) [[code]](https://github.com/RokasEl/simgen)
12. [**ControlMol**, *arXiv 2024*] ControlMol: Adding Substructure Control To Molecule Diffusion Models [[paper]](https://arxiv.org/pdf/2405.06659)
13. [**LDM-3DG**, *ICLR 2024*] Latent 3D Graph Diffusion [[paper]](https://openreview.net/pdf?id=cXbnGtO0NZ) [[code]](https://github.com/Shen-Lab/LDM-3DG)
14. [**CGD**, *ICML 2024*] Context-Guided Diffusion for Out-of-Distribution Molecular and Protein Design [[paper]](https://arxiv.org/pdf/2407.11942) [[code]](https://github.com/leojklarner/context-guided-diffusion)
15. [**END**, *NeurIPS 2024*] Equivariant Neural Diffusion for Molecule Generation [[paper]](https://openreview.net/pdf?id=40pE5pFhWl) [[code]](https://github.com/frcnt/equivariant-neural-diffusion)
16. [**GFMDiff**, *AAAI 2024*] Geometric-Facilitated Denoising Diffusion Model for 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2401.02683)
17. [**MuDM**, *ICLR 2024*] Training-free Multi-objective Diffusion Model for 3D Molecule Generation [[paper]](https://openreview.net/pdf?id=X41c4uB4k0)
18. [**EQGAT-diff**, *ICLR 2024*] Navigating the Design Space of Equivariant Diffusion-Based Generative Models for De Novo 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2309.17296)
19. [**GeoBFN**, *ICLR 2024*] Unified Generative Modeling of 3D Molecules with Bayesian Flow Networks [[paper]](https://openreview.net/pdf?id=NSVtmmzeRB) [[code]](https://github.com/AlgoMole/GeoBFN)
20. [**GruM**, *ICML 2024*] Graph Generation with Diffusion Mixture [[paper]](https://arxiv.org/pdf/2302.03596) [[code]](https://github.com/harryjo97/GruM)
21. [**TACS**, *NeurIPS 2024*] Conditional Synthesis of 3D Molecules with Time Correction Sampler [[paper]](https://openreview.net/pdf?id=gipFTlvfF1)
22. [**FuncMol**, *NeurIPS 2024*] Score-based 3D molecule generation with neural fields [[paper]](https://openreview.net/pdf?id=9lGJrkqJUw) [[code]](https://github.com/prescient-design/funcmol)
23. [**NExT-Mol**, *ICLR 2025*] NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2502.12638) [[code]](https://github.com/acharkq/NExT-Mol)
24. [**ChemGuide**, *ICLR 2025*] Chemistry-Inspired Diffusion with Non-Differentiable Guidance [[paper]](https://openreview.net/pdf?id=4dAgG8ma3B) [[code]](https://github.com/A-Chicharito-S/ChemGuide)
25. [**FMG**, *ICLR 2025*] E(3)-equivariant models cannot learn chirality: Field-based molecular generation [[paper]](https://openreview.net/pdf?id=mXHTifc1Fn) [[code]](https://github.com/Dumitrescu-Alexandru/FMG)
26. [**GOAT**, *ICLR 2025*] Accelerating 3D Molecule Generation via Jointly Geometric Optimal Transport [[paper]](https://openreview.net/pdf?id=VGURexnlUL) [[code]](https://github.com/WanyuGroup/ICLR2025-GOAT)
27. [**ADiT**, *ICML 2025*] All-atom Diffusion Transformers: Unified generative modelling of molecules and materials [[paper]](https://openreview.net/pdf?id=89QPmZjIhv) [[code]](https://github.com/facebookresearch/all-atom-diffusion-transformer)
28. [**IDFlow**, *ICML 2025*] Energy-Based Flow Matching for Generating 3D Molecular Structure [[paper]](https://openreview.net/pdf?id=hcJWWC82KW) [[code]](https://github.com/CaviarLover/IDFlow)
29. [**GeoRCG**, *ICML 2025*] Geometric Representation Condition Improves Equivariant Molecule Generation [[paper]](https://openreview.net/pdf?id=79O2XccGXZ) [[code]](https://github.com/GraphPKU/GeoRCG)
30. [**RADM**, *ICML 2025*] Scalable Non-Equivariant 3D Molecule Generation via Rotational Alignment [[paper]](https://openreview.net/pdf?id=l5KpQ5MmaD) [[code]](https://github.com/skeletondyh/RADM)
31. [**MolTD**, *NeurIPS 2025*] Accelerating 3D Molecule Generative Models with Trajectory Diagnosis [[paper]](https://openreview.net/pdf?id=ATewcZPbDj) [[code]](https://github.com/GenSI-THUAIR/MolTD)
32. [**SLDM**, *NeurIPS 2025*] Straight-Line Diffusion Model for Efficient 3D Molecular Generation [[paper]](https://openreview.net/pdf?id=waHF2ekuf2) [[code]](https://github.com/fengshikun/SLDM)
33. [**UAE-3D**, *NeurIPS 2025*] Towards Unified and Lossless Latent Space for 3D Molecular Latent Diffusion Modeling [[paper]](https://openreview.net/pdf?id=g2XE40zTrj) [[code]](https://github.com/lyc0930/UAE-3D)
34. [**RL-Diffusion**, *NeurIPS 2025*] Uncertainty-Aware Multi-Objective Reinforcement Learning-Guided Diffusion Models for 3D De Novo Molecular Design [[paper]](https://openreview.net/pdf?id=lu4cGylISh) [[code]](https://github.com/Kyle4490/RL-Diffusion)
35. [**SynCoGen**, *ICLR 2026*] SynCoGen: Synthesizable 3D Molecule Generation via Joint Reaction and Coordinate Modeling [[paper]](https://openreview.net/pdf?id=24QKU4iqft) [[code]](https://github.com/andreirekesh/SynCoGen)

### 2D\&3D Molecular Generation

1. [**MolDiff**, *ICML 2023*] MolDiff: Addressing the Atom-Bond Inconsistency Problem in 3D Molecule Diffusion Generation [[paper]](https://arxiv.org/pdf/2305.07508) [[code]](https://github.com/pengxingang/MolDiff)
2. [**MiDi**, *ECML 2023*] MiDi: Mixed Graph and 3D Denoising Diffusion for Molecule Generation [[paper]](https://arxiv.org/pdf/2302.09048) [[code]](https://github.com/cvignac/MiDi)
3. [**MUDiff**, *LoG 2023*] MUDiff: Unified Diffusion for Complete Molecule Generation [[paper]](https://arxiv.org/pdf/2304.14621) [[code]](https://github.com/WillHua127/mudiff)
4. [**JODO**, *TNNLS 2024*] Learning Joint 2-D and 3-D Graph Diffusion Models for Complete Molecule Generation [[paper]](https://arxiv.org/pdf/2305.12347) [[code]](https://github.com/GRAPH-0/JODO)

## Structure-based Drug Design

1. [**TargetDiff**, *ICLR 2023*] 3D Equivariant Diffusion for Target-Aware Molecule Generation and Affinity Prediction [[paper]](https://arxiv.org/pdf/2303.03543) [[code]](https://github.com/guanjq/targetdiff)
2. [**DiffSBDD**, *Nature Computational Science 2024*] Structure-based drug design with equivariant diffusion models [[paper]](https://arxiv.org/pdf/2210.13695) [[code]](https://github.com/arneschneuing/DiffSBDD)
3. [**DecompDiff**, *ICML 2023*] DecompDiff: Diffusion Models with Decomposed Priors for Structure-Based Drug Design [[paper]](https://arxiv.org/pdf/2403.07902) [[code]](https://github.com/bytedance/DecompDiff)
4. [**D3FG**, *NeurIPS 2023*] Functional-Group-Based Diffusion for Pocket-Specific Molecule Generation and Elaboration [[paper]](https://openreview.net/pdf?id=lRG11M91dx)
5. [**LDM-3DG**, *ICLR 2024*] Latent 3D Graph Diffusion [[paper]](https://openreview.net/pdf?id=cXbnGtO0NZ) [[code]](https://github.com/Shen-Lab/LDM-3DG)
6. [**IPDiff**, *ICLR 2024*] Protein-Ligand Interaction Prior for Binding-aware 3D Molecule Diffusion Models [[paper]](https://openreview.net/pdf?id=qH9nrMNTIW) [[code]](https://github.com/YangLing0818/IPDiff?tab=readme-ov-file)
7. [**EQGAT-diff**, *ICLR 2024*] Navigating the Design Space of Equivariant Diffusion-Based Generative Models for De Novo 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2309.17296)
8. [**PMDM**, *Nature Communications 2024*] A dual diffusion model enables 3D molecule generation and lead optimization based on target pockets [[paper]](https://www.nature.com/articles/s41467-024-46569-1) [[code]](https://github.com/Layne-Huang/PMDM?tab=readme-ov-file#pmdm-a-dual-diffusion-model-enables-3d-binding-bioactive-molecule-generation-and-lead-optimization-given-target-pockets)
9. [**BindDM**, *AAAI 2024*] Binding-Adaptive Diffusion Models for Structure-Based Drug Design [[paper]](https://arxiv.org/pdf/2402.18583) [[code]](https://github.com/YangLing0818/BindDM)
10. [**IRDiff**, *ICML 2024*] Interaction-based Retrieval-augmented Diffusion Models for Protein-specific 3D Molecule Generation [[paper]](https://openreview.net/pdf?id=eejhD9FCP3) [[code]](https://github.com/YangLing0818/IRDiff)
11. [**SBE-Diff**, *ICML 2024*] Rethinking specificity in SBDD: Leveraging delta score and energy-guided diffusion [[paper]](https://arxiv.org/pdf/2403.12987)
12. [**MolCRAFT**, *ICML 2024*] MolCRAFT: Structure-Based Drug Design in Continuous Parameter Space [[paper]](https://openreview.net/pdf?id=KaAQu5rNU1) [[code]](https://github.com/AlgoMole/MolCRAFT)
13. [**VoxBind**, *ICML 2024*] Structure-based drug design by denoising voxel grids [[paper]](https://openreview.net/pdf?id=K3fEkECWgu)
14. [**AliDiff**, *NeurIPS 2024*] Aligning Target-Aware Molecule Diffusion Models with Exact Energy Optimization [[paper]](https://arxiv.org/pdf/2407.01648) [[code]](https://github.com/MinkaiXu/AliDiff)
15. [**FlexSBDD**, *NeurIPS 2024*] FlexSBDD: Structure-Based Drug Design with Flexible Protein Modeling [[paper]](https://openreview.net/pdf?id=4AB54h21qG) [[code]](https://github.com/zaixizhang/FlexSBDD)
16. [**DualDiff**, *NeurIPS 2024*] Reprogramming Pretrained Target-Specific Diffusion Models for Dual-Target Drug Design [[paper]](https://openreview.net/pdf?id=Y79L45D5ts) [[code]](https://github.com/zhouxiangxin1998/DualDiff)
17. [**UniGuide**, *NeurIPS 2024*] Unified Guidance for Geometry-Conditioned Molecular Generation [[paper]](https://openreview.net/pdf?id=HeoRsnaD44)
18. [**DrugFlow**, *ICLR 2025*] Multi-domain Distribution Learning for De Novo Drug Design [[paper]](https://openreview.net/pdf?id=g3VCIM94ke) [[code]](https://github.com/LPDI-EPFL/DrugFlow)
19. [**MultiRewardSBDD**, *ICML 2025*] Enhancing Ligand Validity and Affinity in Structure-Based Drug Design with Multi-Reward Optimization [[paper]](https://openreview.net/pdf?id=gmFeso9sXJ)
20. [**UniMoMo**, *ICML 2025*] UniMoMo: Unified Generative Modeling of 3D Molecules for De Novo Binder Design [[paper]](https://openreview.net/pdf?id=KUN7A7Okb6) [[code]](https://github.com/kxz18/UniMoMo)
21. [**CGFlow**, *ICML 2025*] Compositional Flows for 3D Molecule and Synthesis Pathway Co-design [[paper]](https://openreview.net/pdf?id=4aXfSLfM0Z)
22. [**FuncBind**, *NeurIPS 2025*] Unified all-atom molecule generation with neural fields [[paper]](https://openreview.net/pdf?id=JMq90N6lLe) [[code]](https://github.com/prescient-design/funcbind)
23. [**CByG**, *NeurIPS 2025*] Controllable 3D Molecular Generation for Structure-Based Drug Design Through Bayesian Flow Networks and Gradient Integration [[paper]](https://openreview.net/pdf?id=biM1m6VXSD)
24. [**PAFlow**, *NeurIPS 2025*] Prior-Guided Flow Matching for Target-Aware Molecule Design with Learnable Atom Number [[paper]](https://openreview.net/pdf?id=yh1t1yFtXG) [[code]](https://github.com/CMACH508/PAFlow)

## Molecular Docking

1. [**DiffDock**, *ICLR 2023*] DiffDock: Diffusion Steps, Twists, and Turns for Molecular Docking [[paper]](https://arxiv.org/pdf/2210.01776) [[code]](https://github.com/gcorso/DiffDock)
2. [**DynamicBind**, *Nature Communications 2024*] DynamicBind: predicting ligand-specific protein-ligand complex structure with a deep equivariant generative model [[paper]](https://www.nature.com/articles/s41467-024-45461-2) [[code]](https://github.com/luwei0917/DynamicBind)
3. [**Re-Dock**, *ICML 2024*] Re-Dock: Towards Flexible and Realistic Molecular Docking with Diffusion Bridge [[paper]](https://arxiv.org/pdf/2402.11459)
4. [**FMA-PO**, *NeurIPS 2025*] Template-Guided 3D Molecular Pose Generation via Flow Matching and Differentiable Optimization [[paper]](https://openreview.net/pdf?id=cIYguQc97T)
5. [**SigmaDock**, *ICLR 2026*] SigmaDock: Untwisting Molecular Docking with Fragment-Based SE(3) Diffusion [[paper]](https://openreview.net/pdf?id=Vgm77U4ojX) [[code]](https://github.com/alvaroprat97/sigmadock)


## Molecular Optimization

1. [**DiffHopp**, *arXiv 2023*] DiffHopp: A Graph Diffusion Model for Novel Drug Design via Scaffold Hopping [[paper]](https://arxiv.org/pdf/2308.07416) [[code]](https://github.com/jostorge/diffusion-hopping)
2. [**TurboHopp**, *NeurIPS 2023*] TurboHopp: Accelerated Molecule Scaffold Hopping with Consistency Models [[paper]](https://arxiv.org/pdf/2410.20660) [[code]](https://github.com/orgw/TurboHopp)
3. [**PMDM**, *Nature Communications 2024*] A dual diffusion model enables 3D molecule generation and lead optimization based on target pockets [[paper]](https://www.nature.com/articles/s41467-024-46569-1) [[code]](https://github.com/Layne-Huang/PMDM)
4. [**DecompOpt**, *ICLR 2024*] DecompOpt: Controllable and Decomposed Diffusion Models for Structure-based Molecular Optimization [[paper]](https://arxiv.org/pdf/2403.13829) [[code]](https://github.com/bytedance/DecompOpt)
5. [**DiffSBDD**, *Nature Computational Science 2024*] Structure-based drug design with equivariant diffusion models [[paper]](https://arxiv.org/pdf/2210.13695) [[code]](https://github.com/arneschneuing/DiffSBDD)
6. [**ShEPhERD**, *ICLR 2025*] ShEPhERD: Diffusing shape, electrostatics, and pharmacophores for bioisosteric drug design [[paper]](https://openreview.net/pdf?id=KSLkFYHlYg) [[code]](https://github.com/coleygroup/shepherd)
7. [**MolJO**, *ICML 2025*] Empower Structure-Based Molecule Optimization with Gradient Guided Bayesian Flow Networks [[paper]](https://openreview.net/pdf?id=CIoBEB17FT) [[code]](https://github.com/AlgoMole/MolCRAFT)
8. [**MolEditRL**, *ICLR 2026*] MolEditRL: Structure-Preserving Molecular Editing via Discrete Diffusion and Reinforcement Learning [[paper]](https://openreview.net/pdf?id=40QphlZ9fY)


## Conformer Generation

1. [**GeoDiff**, *ICLR 2022*] GeoDiff: a Geometric Diffusion Model for Molecular Conformation Generation [[paper]](https://arxiv.org/pdf/2203.02923) [[code]](https://github.com/MinkaiXu/GeoDiff)
2. [**Torsional Diffusion**, *NeurIPS 2022*] Torsional Diffusion for Molecular Conformer Generation [[paper]](https://arxiv.org/pdf/2206.01729) [[code]](https://github.com/gcorso/torsional-diffusion)
3. [**DiSCO**, *AAAI 2024*] DiSCO: Diffusion Schrödinger Bridge for Molecular Conformer Optimization [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/29238) [[code]](https://github.com/DanyeongLee/DiSCO)
4. [**MCF**, *ICML 2024*] Swallowing the Bitter Pill: Simplified Scalable Conformer Generation [[paper]](https://arxiv.org/pdf/2311.17932) [[code]](https://github.com/apple/ml-mcf)
5. [**ET-Flow**, *NeurIPS 2024*] ET-Flow: Equivariant Flow-Matching for Molecular Conformer Generation [[paper]](https://openreview.net/pdf?id=avsZ9OlR60) [[code]](https://github.com/shenoynikhil/ETFlow)
6. [**EBD**, *NeurIPS 2024*] Equivariant Blurring Diffusion for Hierarchical Molecular Conformer Generation [[paper]](https://openreview.net/pdf?id=Aj0Zf28l6o) [[code]](https://github.com/Shen-Lab/EBD)
7. [**NExT-Mol**, *ICLR 2025*] NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation [[paper]](https://arxiv.org/pdf/2502.12638) [[code]](https://github.com/acharkq/NExT-Mol)
8. [**AvgFlow**, *ICML 2025*] Efficient Molecular Conformer Generation with SO(3)-Averaged Flow Matching and Reflow [[paper]](https://openreview.net/pdf?id=6uPcJtMgWN)
9. [**DiTMC**, *NeurIPS 2025*] Sampling 3D Molecular Conformers with Diffusion Transformers [[paper]](https://openreview.net/pdf?id=tmbx9zGVWb) [[code]](https://github.com/ML4MolSim/dit_mc)


## Linker Design

1. [**DiffLinker**, *Nature Machine Intelligence 2024*] Equivariant 3D-conditional diffusion model for molecular linker design [[paper]](https://arxiv.org/pdf/2210.05274) [[code]](https://github.com/igashov/DiffLinker)


## Molecular Structure Elucidation

1. [**DiffSpectra**, *arXiv 2025*] DiffSpectra: Molecular Structure Elucidation from Spectra using Diffusion Models [[paper]](https://arxiv.org/pdf/2507.06853) [[code]](https://github.com/AzureLeon1/DiffSpectra)
2. [**DiffMS**, *ICML 2025*] DiffMS: Diffusion Generation of Molecules Conditioned on Mass Spectra [[paper]](https://openreview.net/pdf?id=EvILcv2v8L) [[code]](https://github.com/coleygroup/DiffMS)
3. [**ChefNMR**, *NeurIPS 2025*] Atomic Diffusion Models for Small Molecule Structure Elucidation from NMR Spectra [[paper]](https://openreview.net/pdf?id=STsjfx2cee) [[code]](https://github.com/ml-struct-bio/chefnmr)


## Transition State Generation

1. [**OA-ReactDiff**, *Nature Computational Science 2023*] Accurate Transition State Generation with an Object-Aware Equivariant Elementary Reaction Diffusion Model [[paper]](https://www.nature.com/articles/s43588-023-00563-7) [[code]](https://github.com/chenruduan/OAReactDiff)


## Retrosynthesis Prediction and Planning

1. [**RetroDiff**, *AISTATS 2025*] RetroDiff: Retrosynthesis as Multi-stage Distribution Interpolation [[paper]](https://arxiv.org/pdf/2311.14077)
2. [**GDiffRetro**, *AAAI 2025*] GDiffRetro: Retrosynthesis Prediction with Dual Graph Enhanced Molecular Representation and Diffusion Generation [[paper]](https://arxiv.org/pdf/2501.08001) [[code]](https://github.com/sunshy-1/GDiffRetro)
3. [**DiffAlign**, *ICLR 2025*] Equivariant Denoisers Cannot Copy Graphs: Align Your Graph Diffusion Models [[paper]](https://openreview.net/pdf?id=onIro14tHv) [[code]](https://github.com/Aalto-QuML/DiffAlign)


## Molecular Representation Learning

1. [**MoleculeSDE**, *ICML 2023*] A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal Pretraining [[paper]](https://arxiv.org/pdf/2305.18407) [[code]](https://github.com/chao1224/MoleculeSDE)
2. [**MoleculeJAE**, *NeurIPS 2023*] Molecule Joint Auto-Encoding: Trajectory Pretraining with 2D and 3D Diffusion [[paper]](https://openreview.net/pdf?id=xzmaFfw6oh) [[code]](https://github.com/chao1224/Geom3D)
3. [**SubGDiff**, *NeurIPS 2024*] SubGDiff: A Subgraph Diffusion Model to Improve Molecular Representation Learning [[paper]](https://arxiv.org/pdf/2405.05665) [[code]](https://github.com/IDEA-XL/SubgDiff)
4. [**UniGEM**, *ICLR 2025*] UniGEM: A Unified Approach to Generation and Property Prediction for Molecules [[paper]](https://arxiv.org/pdf/2410.10516) [[code]](https://github.com/fengshikun/UniGEM)


## Cite Us

Please feel free to cite this work if you find it helpful!

```
@article{wang2025survey,
  title={Diffusion Models for Molecules: A Survey of Methods and Tasks},
  author={Liang Wang and Chao Song and Zhiyuan Liu and Yu Rong and Qiang Liu and Shu Wu and Liang Wang},
  journal={arXiv},
  volume={abs/2502.09511},
  year={2025}
}
```

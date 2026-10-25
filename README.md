# Research data supporting "Amorphous materials as a frontier challenge for universal interatomic potentials"

This repository supports the manuscript:

> Natascia L. Fragapane and Volker L. Deringer, *"Amorphous materials as a frontier challenge for universal interatomic potentials"* (in preparation).

# AM26 dataset

This repository contains the **AM26** benchmark dataset used to evaluate pre-trained MLIPs for amorphous materials.

The benchmark comprises 5 amorphous systems, together with reference density-functional theory (DFT) energies and forces, spanning a diverse range of chemistries and bonding environments.

The AM26 dataset is available in the [`data`](./data/) directory, both as a combined extxyz file (`am26.extxyz`) and as five separate files for each amorphous system.

Structures included in the AM26 dataset were created using melt-quench simulations for the following systems:
> **a-C**: Melt-quenched structures (1.5–3.5 g cm<sup>−3</sup>) generated using the [C-GAP-17](https://doi.org/10.1103/PhysRevB.95.094203) model.

> **a-SiO<sub>2</sub>**: Melt-quenched structures (quench rates 10<sup>11</sup>–10<sup>14</sup> K s<sup>−1</sup>) generated using the [SiO<sub>x</sub>-ACE-24](https://doi.org/10.1038/s41467-024-45840-9) model.

> **a-LiPS**: Melt-quenched structures spanning compositions along the Li<sub>2</sub>S–P<sub>2</sub>S<sub>5</sub> tie-line, generated using the model of N. L. Fragapane, V. L. Deringer, *J. Chem. Theory Comput.* **2026**, *22*, 3646-3659 [[link](https://doi.org/10.1021/acs.jctc.5c02006)].

Structures were taken from previous work for the following systems:
> **a-Si**: Filtered subset of the a-Si-24 dataset from L. A. M. Rosset, D. A. Drabold, and V. L. Deringer, *Nat. Commun.* **2025**, *16*, 2360 [[link](https://doi.org/10.1038/s41467-025-57406-4)].

> **a-GST**: Combination of AIMD configurations from GST-GAP-22 and the external validation set spanning compositions along the GeTe–Sb<sub>2</sub>Te<sub>3</sub> tie-line: see Y. Zhou, W. Zhang, E. Ma, V. L. Deringer, *Nat. Electron.* **2023**, *6*, 746-754 [[link](https://doi.org/10.1038/s41928-023-01030-x)]. 


# Analysis

We provide the scripts used to reproduce the benchmark error analysis and leaderboard presented in Fig. 2 of the manuscript in the [`scripts`](./scripts/) directory.

These scripts compute prediction errors with respect to the DFT reference data, evaluate the corresponding relative root-mean-square error (RelRMSE) scores, and generate the summary figures used for the benchmark analysis.

# Repository status

This repository will be expanded as additional data and analysis associated with the manuscript become publicly available.

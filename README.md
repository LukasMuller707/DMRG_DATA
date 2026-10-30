# DMRG_DATA
DMRG data supporting the manuscript "Spin-singlet superconductivity driven by bond dimerization in a one-dimensional extended Hubbard model".
Authors: Saisai He, Xichen Huang, Jize Zhao, and Zhong-Bing Huang.
Contact: zhaojz@lzu.edu.cn

This archive contains numerical data supporting Figures 1–7 of the manuscript.


Directory contents:
Figure_1: MATLAB plotting scripts containing phase-boundary coordinates for U = 2 and U = 4.
Figure_2: Correlation functions and local charge densities.
Figure_3: Density structure factor D(k).
Figure_4: Singlet and triplet pairing correlations for different bond combinations.
Figure_5: Pairing correlations for additional parameter sets.
Figure_6: Finite-size scaling data for the density structure factor, used to extract the Luttinger parameter in the thermodynamic limit.
Figure_7: Luttinger parameter, pair binding energy, and spin gap extrapolated to the thermodynamic limit.
File format:
The .d files are plain-text numerical tables with whitespace-separated columns.


Correlation functions and local charge density:
The real-space correlation data are measured within the central region of a system with L = 256, between sites L/4 and 3L/4. The file prefixes identify the observables:
SSF_: Spin-spin correlations.
NNF_: Density-density correlations.
CCF_: Single-particle Green's function.
SINGLET_PAIRING_: Singlet pairing correlations.
TRIPLET_PAIRING_: Triplet pairing correlations.

For the pairing-correlation files in Figures 4 and 5, the prefixes t-t, t-t', and t'-t' identify the bond combinations.
Four-column correlation files: r, i, j, C(i,j), where r is the site separation, i and j are site indices, and C(i,j) is the corresponding correlation function.
Six-column pairing-correlation files: r, i, j, k, l, P(i,j;k,l), where r is the separation between the two bonds, (i,j) and (k,l) specify their endpoints, and P(i,j;k,l) is the corresponding pairing correlation function.
Two-column localChargeDensity files: i, n(i), where i is the site index and n(i) is the local charge density.


Parameters and conventions:
M: DMRG bond dimension.
L: System size.
GQC: Total particle number.
GQS: Twice the total spin quantum number.
T1: Hopping amplitude t.
T2: Hopping amplitude t'.
U: On-site repulsion.
V1: Nearest-neighbor attraction on the t-bonds.
V2: Nearest-neighbor attraction on the t'-bonds.


Software:
The Figure_1 MATLAB scripts use MATLAB R2023b.

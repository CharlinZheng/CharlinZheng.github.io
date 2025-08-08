---
title: Topology-Aware Matrix Partitioning Method for FPGA Real-Time Simulation of Power Electronics Systems
authors:
- Han Xu
- admin
- Yangbin Zeng
- Weicheng Liu
- Fuhai Zhao
- Chunhui Qu
- Zhengming Zhao
author_notes:
- ""
- "Corresponding author"
date: '2023-01-01'
publishDate: '2025-08-07T02:30:46.033636Z'
publication_types: ["article-journal"]
publication: '*IEEE Transactions on Industrial Electronics*'
publication_short: "*IEEE Trans. Ind. Electron.*"
doi: 10.1109/TIE.2023.3308137
abstract: Field-programmable gate array (FPGA)-based real-time simulation serves as a powerful tool for testing and validating power electronics system (PES). However, accurate real-time simulation in high-frequency applications demands extremely small time steps, which poses significant computational and memory challenges. Explicit methods can achieve small time steps due to low-computational burdens, but have stability issues. In this article, the authors propose a topology-aware matrix partitioning (TA-MP) method, which adopts the implicit numerical algorithm to ensure stability, and uses iterative methods to solve the implicit equations. In detail, the PES matrix is partitioned into blocks with clear topological meanings, and its constant diagonal blocks are used to construct a constant iterative matrix. Since the iterative matrix is constant, the TA-MP method bypasses the limitations of using iterative methods in real-time simulations by predetermining the number of iterations. The TA-MP method eliminates the need to store inverse matrices for different topologies, requiring only matrix-vector multiplications, which are efficient on FPGA. The TA-MP method's effectiveness is validated with n-port active bridge converters on an FPGA board with a 25 ns step size, ensuring simulation accuracy at the highest switching frequency of 200 kHz while consuming only 1/15 the memory resources of the conventional method.

tags:
- Power Electronics
- Edge Computing
- Real-time Simulation
featured: false

url_pdf: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10242237
---

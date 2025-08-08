---
title: An Event-Driven Real-Time Simulation for Power Electronics Systems Based on Discrete Hybrid Time-Step Algorithm
authors:
- admin
- Zhengming Zhao
- Yangbin Zeng
- Bochen Shi
- Zhujun Yu
  
date: '2023-05-01'
publishDate: '2025-08-07T02:30:46.116398Z'

publication_types: ["article-journal"]

publication: '*IEEE Transactions on Industrial Electronics*'
publication_short: "*IEEE Trans. Ind. Electron*"

doi: 10.1109/TIE.2022.3187594


abstract: Real-time (RT) hardware-in-the-loop (HIL) simulation aims to speed up the validation process for power electronic systems (PES). The complex PESs with high switching frequency constitute some of the most challenging applications in RT-HIL. Conventional RT-HIL relies on adding extra expensive computing hardware to achieve submicrosecond step size, reducing errors caused by unavoidable sampling delays. This article proposes a CPU-based event-driven RT (EDRT) simulation framework by improving the algorithm rather than using additional hardware. The framework consists of two parts: 1) the synchronous-cycle event detection sampling method, which eliminates the delay error by detecting switching events; and 2) the discrete hybrid time-step numerical algorithm, which combines variable and fixed step-size simulation to improve the calculation efficiency and uses the ideal model to improve the modeling accuracy. The proposed framework is applied to a power electronic transformer with 24 switches and a 20 kHz switching frequency as a simulated case. Comparing the proposed simulation results with experimental results and other simulation results, the proposed EDRT framework can achieve the same numerical accuracy as the offline simulation but only requires 1/36 of the computation time. Furthermore, the hardware cost to achieve the same computational scale is reduced to 1/20 of the conventional HIL.

summary: This paper presents an innovative event-driven real-time simulation framework for power electronic systems, significantly enhancing simulation efficiency and accuracy while reducing hardware costs.

tags:
- Power Electronics
- Real-Time Simulation
- Numerical Methods
featured: false

url_pdf: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9819434

---

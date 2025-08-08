---
title: An Event-Driven Parallel Acceleration Real-Time Simulation for Power Electronic Systems Without Simulation Distortion in Circuit Partitioning
authors:
- admin
- Zhengming Zhao
- Yangbin Zeng
- Shiqi Ji
- Liqiang Yuan
- 
date: '2022-12-01'
publishDate: '2025-08-07T02:30:46.108759Z'

publication_types: ["article-journal"]

publication: '*IEEE Transactions on Power Electronics*'
publication_short: "*IEEE Trans. Power Electron*"

doi: 10.1109/TPEL.2022.3191877

abstract: The trend toward higher switching frequency and larger scale of power electronic systems poses challenges for real-time simulation. This article presents an event-driven hardware-in-the-loop (ED-HIL) simulation framework that does not rely on the small fixed simulation step-size related to the switching frequency. ED-HIL framework can improve the calculation efficiency by positioning switch events and using variable simulation step-size. Further, a parallel acceleration and circuit partitioning (PACP) solver is proposed based on this framework. The PACP solver partitions the circuit with energy storage elements and ensures that the partitioning does not introduce simulation distortion by using the higher order derivatives of the energy storage elements. Meanwhile, it achieves a process-level paralleling through a shared memory architecture in order to accelerate the simulation. As a result, the proposed PACP solver based on the ED-HIL framework can achieve about three times the simulation scale of a commercial FPGA-based real-time simulator at 1 of 16 the hardware cost under the same conditions. An accurate real-time HIL example of a power electronic transformer with 32 switches at a switching frequency of 20 kHz has been implemented on a personal computer. The simulation results are analyzed by comparing with experiment, offline software, and commercial real-time simulator.

summary: This paper introduces an innovative ED-HIL simulation framework and a PACP solver, significantly enhancing the real-time simulation capabilities of power electronic systems.

tags:
- Power Electronics
- Real-Time Simulation
- Numerical Methods
featured: false

url_pdf: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9832797
---

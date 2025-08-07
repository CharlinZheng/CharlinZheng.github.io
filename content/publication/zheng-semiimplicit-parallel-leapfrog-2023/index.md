---
title: A Semi-implicit Parallel Leapfrog Solver with Half-Step Sampling Technique for FPGA-based Real-time HIL Simulation of Power Converters
authors:
- admin
- Yangbin Zeng
- Zhengming Zhao
- Weicheng Liu
- Han Xu
- Shiqi Ji

date:  "2023-04-11T00:00:00Z"
publishDate:  "2024-03-01T02:30:46.170355Z"

publication_types: ["article-journal"]

publication: '*IEEE Transactions on Industrial Electronics*'
publication_short: "*IEEE Trans. Ind. Electron.*"

doi: 10.1109/TIE.2023.3265042

abstract: Field Programmable Gate Array (FPGA) based Hardware-in-the-loop (HIL) simulation is an effective tool to verify the performance of physical controllers and shorten the development cycle of power converters. In HIL simulations, sampling accuracy is of concern and is desired to be improved by reducing the step size. However, due to the cost of computational time, the step size is hard to reduce indefinitely to meet the requirements for high switching frequency applications. To improve the sampling accuracy and simulation performance of HIL simulation, this paper proposes a semi-implicit parallel leapfrog (SPL) solver with half-step sampling technique. In this solver, the switches and the rest part of the system are implemented to be computed parallel when the switch leg model operates in continuous current mode. Besides, the solver is formulated in leapfrog format to reduce computational costs and to compute at half-step as a minimum step-size. With this format, the half-step sampling technique can be employed to increase the sampling rate by onefold, even in cases where it is challenging to reduce the simulation step size further. A dual active bridge converter case is implemented on the FPGA board with a 12.5-ns sampling step-size, retaining the simulation accuracy while switched at 400 kHz. To further verify the advantages, the results are compared with other HIL method and experimental results.

summary: A novel SPL solver improves FPGA-HIL simulation accuracy for high-frequency converters using parallel computation and half-step sampling.

tags:
- Power Electronics
- Edge Computing
featured: false

url_pdf: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10100633

---

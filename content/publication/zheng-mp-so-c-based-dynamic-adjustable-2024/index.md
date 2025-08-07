---
title: MPSoC-Based Dynamic Adjustable Time-Stepping Scheme With Switch Event Oversampling Technique for Real-Time HIL Simulation of Power Converters
authors:
- admin
- Yangbin Zeng
- Zhengming Zhao
- Weicheng Liu
- Han Xu
- Haoyu Wang
- Di Mou
  
date: '2024-06-01'
publishDate: '2025-08-07T02:30:46.146686Z'

publication_types: ["article-journal"]

publication: '*IEEE Transactions on Transportation Electrification*'
publication_short: "*IEEE Trans. Transp. Electr.*"

doi: 10.1109/TTE.2023.3310509

abstract: Hardware-in-the-loop (HIL) simulation is widely used in the design and test process of power converters; however, the conventional fixed-step HIL simulations are accompanied by significantly high computational costs and struggle to accurately locate and calculate switching events in high-frequency applications. This article, therefore, proposes a dynamic adjustable time-stepping (DAT) simulation scheme with a switch event oversampling (SEO) technique. In detail, the SEO technique uses oversampled control signals and simulated modulation processes to predict all switching events information accurately throughout a control cycle. Meanwhile, with the switching events information, the DAT scheme can adjust the simulation time stepping in advance, ensuring simulation accuracy by adjusting the order of the numerical algorithm; furthermore, the iterative calculation can be used to locate the natural commutation of diodes accurately due to the flexible time stepping and order. The global performance and the hardware use of the proposed scheme are evaluated by numerical experiments and HIL experiments in a 32-switches modular multiactive bridge converter with a switching frequency of 400 kHz. The results demonstrate that the proposed scheme can improve the simulation accuracy by 42times while reducing 90% of the computation memory compared with the commercial HIL simulator.


summary: A DAT+SEO scheme boosts HIL simulation accuracy 42× and reduces memory use by 90% through adaptive step-sizing and precise switching event prediction.

tags:
- Power Electronics
- Edge Computing
- Hardware-in-the-loop (HIL)
- Real-time Simulation
featured: false

url_pdf: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10236507
---

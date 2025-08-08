---
title: A Scalable Network-Aware Multi-Agent Reinforcement Learning Framework for Decentralized Inverter-based Voltage Control
authors:
- Han Xu
- admin
- Guannan Qu
date: '2023-12-01'
publishDate: '2025-08-07T02:30:46.018599Z'
publication_types: ["article"]
publication: '*arXiv*'
doi: 10.48550/arXiv.2312.04371
abstract: This paper addresses the challenges associated with decentralized voltage control in power grids due to an increase in distributed generations (DGs). Traditional model-based voltage control methods struggle with the rapid energy fluctuations and uncertainties of these DGs. While multi-agent reinforcement learning (MARL) has shown potential for decentralized secondary control, scalability issues arise when dealing with a large number of DGs. This problem lies in the dominant centralized training and decentralized execution (CTDE) framework, where the critics take global observations and actions. To overcome these challenges, we propose a scalable network-aware (SNA) framework that leverages network structure to truncate the input to the critic's Q-function, thereby improving scalability and reducing communication costs during training. Further, the SNA framework is theoretically grounded with provable approximation guarantee, and it can seamlessly integrate with multiple multi-agent actor-critic algorithms. The proposed SNA framework is successfully demonstrated in a system with 114 DGs, providing a promising solution for decentralized voltage control in increasingly complex power grid systems.


tags:
- Reinforcement Learning
- Multi-Agent Systems
- Systems and Control
- Optimization and Control
featured: false
url_pdf: https://arxiv.org/pdf/2312.04371
---

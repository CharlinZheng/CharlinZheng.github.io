
# 📝 Publications 
So far, my research has focused on Power Electronic Dense Grids (PEDGs) and categorized into five topics. In the future, I hope to do more interesting work in **physics-informed** machine learning for **modeling**, **control** and **optimization** of PEDGs.
- [*01 Digital Twins for PEDG Critical Devices*](#pedg-critical-devices)
- [*02 Deep Machine Learning in PEDGs*](#deep-machine-learning)
- [*03 Edge Computing for PEDG Application*](#edge-computing)
- [*04 Real-Time Simulation and HIL Simulation*](#HIL-simulation)
- [*05 Design and Control of PEDG Converter*](#Desigh-Control)

## 📈 <a id="pedg-critical-devices">Digital Twins for PEDG Critical Devices</a>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans Ind. Informat.</div><img src='images/DigitalTwins01.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

***Cognitive Digital Twins for Model Predictive Control of High-Frequency Power Converters*** (Under Review) \\
**Jialin Zheng**, Haoyu Wang, Yangbin Zeng, Di Mou, et al.

- **First use** of digital twins for model predictive control of high-frequency power converters.
- Get real operating modes and system parameters of the physical converter at the **converter edge**.
- The cognitively obtained information is computed to **enhance** the dynamic performance of the converter.
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Neural Networks Learn. Syst.</div><img src='images/DigitalTwins02.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

***Neural ODE-based Online Modeling of Unknown Power Electronic Systems***(Under Review) \\
**Jialin Zheng**, Haoyu Wang, Yangbin Zeng, Di Mou, et al.
- Directly **neuralizing** the converters' ordinary differential equations (ODEs)，ensuring physical constraints and compatibility with existing ODE-based design and control methods.
- Modeling unknown systems on **local edge devices** to guarantee privacy
- Use **adjoint states** to obtain nearly **constant training cost**, independent of model depth
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Ind. Electron. </div><img src='images/DigitalTwins03.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***Real-Time Digital Mapped Method for Sensorless Multitimescale Operation Condition Monitoring of Power Electronics Systems***](https://ieeexplore.ieee.org/abstract/document/10122863) \\
Y. Zeng, **J. Zheng(Corresponding Author)**, Z. Zhao, W. Liu, S. Ji and H. Li
- **Non-invasive** acquisition of all states inside the converter **without** any kind of sensors
- Across **multiple time scales**, from subtle switching dynamics to second-level voltage fluctuations
- **Signal-level** interaction for safety, convenience, and efficiency
</div>
</div>

- ``IEEE Trans. Transp. Electrif.`` [FPGA-based Real-Time X-in-the-loop Simulation Testbench for Dynamic Wireless Power Transfer System with Stochastic and Nonlinear Inductance](https://ieeexplore.ieee.org/abstract/document/10551289),  **J. Zheng**, Y. Zeng, Z. Zhao, et al.
- ``IEEE Trans. Transp. Electrif.`` [FPGA-Based Implicit–Explicit Real-Time Simulation Solver for Railway Wireless Power Transfer With Nonlinear Magnetic Coupling Components](https://ieeexplore.ieee.org/abstract/document/10318137) Han Xu, Y. Zeng, **J. Zheng**, Z. Zhao, et al.

## 🎙  <a id="deep-machine-learning">Deep Machine Learning in PEDGs</a>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Smart Grid </div><img src='images/MachineLearning01.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***A Scalable Network-Aware Multi-Agent Reinforcement Learning Framework for Decentralized Inverter-based Voltage Control***](https://arxiv.org/abs/2312.04371) \\
Han Xu, **Jialin Zheng**, Guannan Qu
- Using **Localized observation** for critics in the CTDE framework，enhanceing scalability for large-scale PEDGs.
- Truncating Q-function inputs based on **network structure**，reducing communication costs during training significantly.
- **Theoretical guarantees** ensure robust approximation, compatible across diverse multi-agent actor-critic algorithms.
</div>
</div>

## 📚 <a id="edge-computing">Edge Computing for PEDG Application</a> 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Ind. Electron.</div><img src='images/EdgeComputing01.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***A Semi-Implicit Parallel Leapfrog Solver With Half-Step Sampling Technique for FPGA-Based Real-Time HIL Simulation of Power Converters***](https://ieeexplore.ieee.org/abstract/document/10100633) \\
**J. Zheng**, Y. Zeng, Z. Zhao, W. Liu, H. Xu and S. Ji
- A semi-implicit numerical integration scheme, combining the **high parallelism** of explicit methods with the **numerical stability** of implicit methods.
- Leapfrog operation with half-step increments, naturally **doubling the sampling frequency**, applicable across any switching frequency.
- A hierarchical modeling approach that translates topology changes caused by switching actions into input variations, maintaining a **constant system matrix**.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Transp. Electrif.</div><img src='images/EdgeComputing02.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***MPSoC-Based Dynamic Adjustable Time-Stepping Scheme With Switch Event Oversampling Technique for Real-Time HIL Simulation of Power Converters***](https://ieeexplore.ieee.org/abstract/document/10236507) \\
**Jialin Zheng**; Yangbin Zeng; Zhengming Zhao; Weicheng Liu; Han Xu; Haoyu Wang and Di Mou
- An oversampling method where the sampling frequency depends solely on hardware performance, **unaffected by system scale** or algorithm execution time.
- Dynamically adjusts computation step-size, performing calculations **only at critical points.**
- Capable of accurately characterizing all switching actions in multi-active bridge converters at frequencies up to 400 kHz, **far exceeding** the current average of 20 kHz.

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Ind. Electron.</div><img src='images/EdgeComputing03.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***Topology-Aware Matrix Partitioning Method for FPGA Real-Time Simulation of Power Electronics Systems***](https://ieeexplore.ieee.org/abstract/document/10242237) \\
Han Xu, **Jialin Zheng(Corresponding Author)**, Yangbin Zeng, Weicheng Liu, et al.
- Divides the system matrix into blocks with explicit topological significance according to the **topology structure**.
- Constructs a **constant iterative matrix** using its constant diagonal blocks, achieving a fixed iterative matrix and iteration count.
- Utilizes a fully implicit numerical integration method **without the need** to store all matrices or perform indefinite iterative calculations, as required by traditional methods.
</div>
</div>


- ``IEEE Trans. Power Electron.`` [Event-Synchronous Time-Asynchronous Method for Controller HIL Simulation of 10 kVA Modular Multilevel Converters](https://ieeexplore.ieee.org/abstract/document/10128737), Y. Zeng, **J. Zheng(Corresponding Author)**, Z. Zhao, W. Liu, Z. Wang and H. L.
- ``IEEE J. Emerging Sel. Top. Power Electron.`` [Extended Discrete-State Event-Driven Hardware-in-the-Loop Simulation for Power Electronic Systems Based on Virtual-Time-Ratio Regulation](https://ieeexplore.ieee.org/abstract/document/10098796), Yangbin Zeng, Zhengming Zhao, **Jialin Zheng(Corresponding Author)**, Don Tan, Weicheng Liu, et al.
- ``IEEE Access`` [An Adaptive Word-Length Selection Method to Optimize Hardware Resources for FPGA-Based Real-Time Simulation of Power Converters](https://ieeexplore.ieee.org/abstract/document/10302297), Fuhai Zhao, Jiang Du, Yunkai Deng, **Jialin Zheng**, Yangbin Zeng, Chunhui Qu.
- ``ECCE 2023`` [Event-Driven Controller Hardware-In-The-Loop Simulation for Modular Multilevel Converters](https://ieeexplore.ieee.org/abstract/document/10362945), Yangbin Zeng, Weicheng Liu, **Jialin Zheng**, Haoyu Wang, Han Xu, Di Mou, Zhengming Zhao, Hong Li and Zuoxing Wang.

## 🎼 <a id="HIL-simulation">Real-Time Simulation and HIL Simulation</a>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Power Electron</div><img src='images/HIL01.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***An Event-Driven Parallel Acceleration Real-Time Simulation for Power Electronic Systems Without Simulation Distortion in Circuit Partitioning***](https://ieeexplore.ieee.org/abstract/document/9832797) \\
**Jialin Zheng**, Zhengming Zhao, Yangbin Zeng, et al.
- Localized observation for critics in the CTDE framework enhances scalability for systems with numerous DGs.
- Truncated Q-function inputs based on network structure significantly reduce communication costs during training.
- Theoretical guarantees ensure robust approximation, compatible across diverse multi-agent actor-critic algorithms.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Ind. Electron.</div><img src='images/HIL03.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***An Event Driven Synchronization Framework for Physical Controller Co-Simulation of Megawatt-Level Power Electronic Systems***](https://ieeexplore.ieee.org/abstract/document/10242602) \\
**Jialin Zheng**, Yangbin Zeng, Zhengming Zhao, Weicheng Liu, Han Xu, et al.
- Localized observation for critics in the CTDE framework enhances scalability for systems with numerous DGs.
- Truncated Q-function inputs based on network structure significantly reduce communication costs during training.
- Theoretical guarantees ensure robust approximation, compatible across diverse multi-agent actor-critic algorithms.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="font-style: italic;">IEEE Trans. Ind. Electron.</div><img src='images/HIL02.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[***A Self-Restoring Fault-Tolerant Method for Controller Cooperation Simulation of Power Electronics Systems***](https://ieeexplore.ieee.org/abstract/document/10061485) \\
Yangbin Zeng, Zhengming Zhao, **Jialin Zheng(Corresponding Author)**, et al.
- Localized observation for critics in the CTDE framework enhances scalability for systems with numerous DGs.
- Truncated Q-function inputs based on network structure significantly reduce communication costs during training.
- Theoretical guarantees ensure robust approximation, compatible across diverse multi-agent actor-critic algorithms.
</div>
</div>

- ``IEEE Trans. Ind. Electron.`` [An Event-Driven Real-Time Simulation for Power Electronics Systems Based on Discrete Hybrid Time-Step Algorithm](https://ieeexplore.ieee.org/abstract/document/9819434), **Jialin Zheng**, Zhengming Zhao, Yangbin Zeng, et al.
- ``IEEE Trans. Ind. Electron.`` [Numerical Derivative-Based Flexible Integration Algorithm for Power Electronic Systems Simulation Considering Nonlinear Components](https://ieeexplore.ieee.org/abstract/document/10342664), Han Xu, Bochen Shi, Zhujun Yu, **Jialin Zheng**, Zhengming Zhao.
- ``IEEE J. Emerging Sel. Top. Power Electron.`` [Adaptive Synchronization Interface with Key-Frame Prediction Method for Accelerating Power Electronics Co-Simulation](https://ieeexplore.ieee.org/abstract/document/10589637), Weicheng Liu; Zhengming Zhao; Yangbin Zeng; **Jialin Zheng**; Han Xu.
- ``PEDG 2023`` [Topology-aware Iterative Method for Large-scale Power Electronic Systems with Stray Parameters](https://ieeexplore.ieee.org/abstract/document/10215133), Han Xu, Zhengming Zhao, Bochen Shi, Yangbin Zeng, **Jialin Zheng**, Weicheng Liu.
- ``ECCE 2023``  [Multi-rate State-Variable-Interfaced Decoupling Simulation Strategy for Large-Scale Power Electronics Systems](https://ieeexplore.ieee.org/abstract/document/10362779), Han Xu, Zhengming Zhao, Yangbin Zeng, **Jialin Zheng**, Bochen Shi, Weicheng Liu.
- ``PEDG 2023`` [Hybrid Time and Event Co-simulation Framework for Power Electronics Systems](https://ieeexplore.ieee.org/abstract/document/10215222), Weicheng Liu, Zhengming Zhao, Bochen Shi, Yangbin Zeng, **Jialin Zheng**, Han Xu.


## 🧑‍🎨 <a id="Desigh-Control">Design and Control of PEDG Converter</a>
- ``IEEE J. Emerging Sel. Top. Power Electron.`` [Overview of Multi-Degree-of-Freedom Modulation Techniques for Dual Active Bridge Converter](https://ieeexplore.ieee.org/abstract/document/10274900), Di Mou, Liqiang Yuan, Quanming Luo, Yalun Li, Chengwei Liu, **Jialin Zheng** and Zhengming Zhao.
- ``IEEE Trans. Ind. Electron.`` [Universal Phase-Shift Modulation Scheme and Efficiency Optimization for Modular Multiactive Bridge Converter](https://ieeexplore.ieee.org/abstract/document/10242261), Haoyu Wang, Di Mou, Shiqi Ji, Liqiang Yuan, Yangbin Zeng, **Jialin Zheng** and Zhengming Zhao.
- ``ECCE 2023`` [Comparison and Improvement of ZVS Operation Under Different Modulation Strategies for Modular Multi Active Bridge Converters](https://ieeexplore.ieee.org/abstract/document/10362302), Haoyu Wang; Di Mou; Shiqi Ji; Matthias Preindl; Yangbin Zeng; **Jialin Zheng**, Han Xu, Weicheng Liu and Wenhao Xie.
-  ``ECCE 2023`` [A Hybrid Modulation Strategy for the Modular Quad-Active Bridge Converters with the Aid of DC Blocking Capacitors](https://ieeexplore.ieee.org/abstract/document/10362781), Di Mou; Liqiang Yuan; Haoyu Wang; Yangbin Zeng; **Jialin Zheng**; Weicheng Liu

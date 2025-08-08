---
title: "Edge Digital Twins for Power Electronics"
summary: "Sim-to-Real Edge Digital Twins that fuse event-aware physics with neural operators for sub-microsecond inference, online parameter self-calibration, and control integration on FPGA/MPSoC."
tags:
  - ML
  - Modeling
  - Sim
  - Control
  - Edge
date: 2022-01-01
---

{{< youtube wQCjyyNlD6U >}}

## Overview
This project develops **Edge Digital Twins (EDTs)** that run next to converters and inverters to deliver **low-latency, high-fidelity state inference** and **control-ready predictions**. The core idea is to marry the hybrid physics of power electronics (continuous ODEs + discrete switching events) with **neural operators** and a **cloud-to-edge toolchain**, so the twin remains interpretable, fast, and deployable on constrained hardware such as FPGAs and MPSoCs.

## Just Ask for questions！

Explore our research with an AI assistant powered by the latest Gemini models and reliable sources to enhance your understanding and analysis.

<div style="text-align:center; margin: 1rem 0;">
  <a href="https://notebooklm.google.com/notebook/c79438f8-198a-4754-b174-67aade45c1a1"
     class="btn btn-primary btn-lg"
     target="_blank" rel="noopener">
    Start exploring
  </a>
</div>


## Why This Research
- **Real-time pressure at the edge.** High-frequency converters (100 kHz–MHz) impose **sub-µs** compute budgets; generic sampling-based twins are too slow or too coarse to capture switching events precisely.  
- **Sim-to-Real gap.** Pure physics models drift under unmodeled effects; pure data models need huge datasets and struggle with mode transitions—both hinder **trustworthy control integration**.  
- **Hardware constraints.** Variable-step high-order solvers are accurate but **sequential** and time-uncertain on FPGAs; fixed-step solvers are parallel but **computationally explosive**.  
- **Control needs visibility.** Advanced control (e.g., MPC) benefits from **global state** without adding sensors or latency; this requires a twin that is **accurate, adaptable, and fast** at the edge.
{{< figure src="hardware.jpg" caption="Edge Digital Twins Platform" numbered="true" >}}

## New Measures
- **Physics-Embedded Neural ODE (PENODE).** Event-aware **mode automata** drive per-mode continuous-time **neural ODEs** that inject known ODE primitives as **physics priors** and learn only residual dynamics. This preserves interpretability, improves data efficiency, and supports adaptive integration.  
{{< figure src="penode.jpg" caption="Physics-Embedded Neural ODE Modeling" numbered="true" >}}
- **Neural Substitute Solver (NSS).** A dual-NN design replaces (i) **online model updates** tied to switching events and (ii) **higher-order truncation terms** of base integrators—turning sequential bottlenecks into **parallel forward passes** suitable for FPGA/MPSoC.  
{{< figure src="nss.jpg" caption="Neural Substitute Solver Architecture" numbered="true" >}}
- **Cognitive DT for Control (CDT-MPC).** A **mode-driven variable-order solver** plus **LM-based parameter identification** yields a reconfigurable numerical twin that supplies **sensor-free global states** to MPC, enabling **dead-beat** responses without high-bandwidth probes.  
- **Cloud-to-Edge toolchain.** Quantization, operator fusion, and **neural processing units** (NPUs) map PENODE/NSS/CDT to edge hardware with consistent real-time guarantees.

## Impact
- **Speed & resources.** Edge inference speedups (e.g., **>20×**) with **>50%** compute/resource savings vs. traditional solvers, meeting **sub-µs** deadlines for high-frequency operation.  
- **Fidelity & robustness.** Physics-guided residual learning improves Sim-to-Real generalization and maintains accuracy across **white/gray/black-box** regimes; online LM identification tracks parameter drift.  
- **Control performance.** CDT-MPC achieves **dead-beat transients**, eliminates sensor sampling delays, and expands MPC candidate sets without manual derivations—improving dynamic response and stability margins.  
- **Deployability.** Event-aware scheduling + precomputed per-mode matrices + parallel NN operators enable stable timing on **FPGA/MPSoC**, easing field integration.  
- **Generality.** Applicable from single converters to **multi-port, multi-converter** systems; modular design supports future addition of observers, fault diagnosis, and fleet-level coordination.

## Publications

{{< cite page="/publication/zheng-physics-embedded-neural-od-es-2025" view=1 >}}
{{< cite page="/publication/zheng-neural-substitute-solver-2025" view=1 >}}
{{< cite page="/publication/zheng-cognitive-digital-twins-based-2025" view=1 >}}




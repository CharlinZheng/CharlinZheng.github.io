---
title: "Hybrid Dynamical System Modeling and Inference via Machine Learning"
summary: "A unified ML framework—Event-Automata + Physics-Embedded Neural ODEs + Neural Substitute Solver—for accurate, real-time inference of hybrid (continuous–discrete) dynamics with reliable Sim-to-Real transfer to edge hardware."

tags:
  - ML
  - Modeling
  - Sim
  - Control
  - Edge
date: 2025-01-01
---

{{< youtube -_JWBCtUf_8 >}}

## Overview
This project tackles the core difficulty of **hybrid dynamical systems** in power electronics: **continuous ODE evolution punctuated by discrete switching events**. We design models that (i) explicitly recognize **event/mode structure**, (ii) **embed physics** to reduce data burden and preserve interpretability, and (iii) run **fast enough at the edge** to support control. The result is a practical stack for **modeling, inference, and control** that remains stable under mode transitions and robust in Sim-to-Real deployment.

## Just Ask for questions！

Explore our research with an AI assistant powered by the latest Gemini models and reliable sources to enhance your understanding and analysis.

<div style="text-align:center; margin: 1rem 0;">
  <a href="https://notebooklm.google.com/notebook/58f97af1-c852-4118-834e-abb18429f867"
     class="btn btn-primary btn-lg"
     target="_blank" rel="noopener">
    Start exploring
  </a>
</div>


## Why This Research
- **Hybrid dynamics are hard to learn.** Standard discrete networks conflate sampling with dynamics and struggle with irregular mode durations.  
- **Sim-to-Real is brittle.** Pure physics breaks under parameter drift; pure black-box needs huge data and often fails at mode boundaries.  
- **Edge devices are resource-constrained.** Real-time requirements (sub-µs) and tight memory make classic high-order solvers impractical.  
- **Goal.** Build **event-aware, physics-consistent, edge-deployable** models that keep continuous-time fidelity, cross mode transitions cleanly, and meet hard latency budgets.

## New Measures
- **Event-Automata Learning (EA).** Decode control/PWM into **mode sequences** and **event times**, then learn per-mode dynamics; avoids sampling delay and reduces learning interference across modes.  
- **Physics-Embedded Neural ODEs (PENODE).** Parameterize the continuous-time vector field as **f(x,u)=f_phy(x,u;θ_phy)+f_NN(x;θ_NN)**. Physics supplies a stable backbone; the NN learns residuals only—improving data efficiency, interpretability, and generalization.  
- **Neural Substitute Solver (NSS).** Replace two bottlenecks in numerical solvers with lightweight NNs: (1) **event-triggered model updates** (matrix ops) and (2) **higher-order truncation terms** of the integrator—turning sequential steps into parallel forward passes suitable for FPGA/MPSoC.  
- **Unified training with adjoint/backprop.** Jointly optimize physical parameters and NN weights end-to-end; supports white-, gray-, and black-box regimes with a single pipeline.  
- **Cloud→Edge toolchain.** Quantization-aware training, operator fusion, and HLS-based accelerators map PENODE/NSS to **FPGAs/MPSoCs** with deterministic timing; EA provides event-driven scheduling at inference.  
- **Data program for Sim-to-Real.** Curate mixed **simulation + hardware** traces across modes and operating ranges; use EA to segment/align trajectories, then fine-tune to the target plant with small data.

## Impact
- **Learning efficiency.** Event-aware decomposition reduces model size and accelerates convergence compared with single-mode discrete nets; residual learning lowers data demand.  
- **Sim-to-Real reliability.** Physics-anchored representations maintain accuracy under parameter drift and unseen conditions; unified training avoids two-stage inconsistencies.  
- **Real-time edge inference.** NSS and compact PENODE kernels deliver consistent per-step latency with low resource use—suitable for sub-µs budgets.  
- **Control integration.** Continuous-time states/derivatives and clean mode boundaries feed MPC/optimal control without ad-hoc filters; improved transients and stability margins.  
- **Maintainability & insight.** Physical parameters remain visible and tunable; residual terms highlight unmodeled effects for diagnostics.


## Publications

{{< cite page="/publication/zheng-physics-embedded-neural-od-es-2025" view=1 >}}
{{< cite page="/publication/zheng-neural-substitute-solver-2025" view=1 >}}




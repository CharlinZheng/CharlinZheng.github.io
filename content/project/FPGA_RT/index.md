---
title: "Sub-Microsecond Real-Time FPGA Numerical Solver"
summary: "Deterministic sub-µs FPGA solvers (12.5–75 ns) combining semi-implicit leapfrog, topology-aware partitioning, and IMEX techniques for stability, low memory, and controller-accurate HIL."



tags:
  - Modeling
  - Sim
  - Edge
date: 2022-01-01
---
{{< youtube ijgKofb23cA >}}

## Overview
This project develops **numerical solvers for FPGA-based real-time simulation** that meet **sub-microsecond** deadlines without sacrificing accuracy or stability. We target high-frequency, switch-dense converters where traditional explicit solvers become unstable and implicit solvers exceed FPGA latency/memory limits. Our designs guarantee **fixed computation time per step**, preserve **switch-level fidelity** (two-state models), and support **nonlinear/stochastic** components needed for realistic controller testing. 

## Just Ask for questions！

Explore our research with an AI assistant powered by the latest Gemini models and reliable sources to enhance your understanding and analysis.

<div style="text-align:center; margin: 1rem 0;">
  <a href="https://notebooklm.google.com/notebook/f9772ebe-a49c-4188-a3fc-f9f24f4347c5"
     class="btn btn-primary btn-lg"
     target="_blank" rel="noopener">
    Start exploring
  </a>
</div>


## Why This Research
- **Hard real-time at MHz-class switching.** Accurate HIL often needs steps ≤1/50–1/100 of the switching period; with wide-bandgap devices this pushes into **tens of nanoseconds**—beyond what sequential matrix factorizations on FPGAs can deliver.
- **Implicit vs. memory.** Storing per-topology inverses improves latency but explodes **FPGA memory** and scales poorly with switch count. We need implicit-level stability **without** inverse storage.
- **Nonlinear & stochastic reality.** Wireless power transfer and dynamic environments induce **nonlinear magnetic coupling** and **stochastic parameter drift**—capabilities rarely supported together in RT HIL.
- **Sampling fidelity.** Even if the step cannot shrink further, **higher sampling rate** is essential to capture PWM edges and avoid duty-cycle bias. 

## New Measures
- **Semi-Implicit Parallel Leapfrog (SPL) + Half-Step Sampling.** A hierarchical parallel equivalent (HPE) model separates switch- and system-levels; an **alternating implicit integration** leapfrog reduces cost and **enables half-step sampling** (2× sampling rate) while keeping stability. Demonstrated at **12.5 ns** per sample on a DAB at **400 kHz**.
- **Topology-Aware Matrix Partitioning (TA-MP).** Partitions the system along switching legs and builds a **constant iterative matrix** for implicit solves—**no per-topology inverses**, **fixed iteration count** per step. Achieves **25 ns** step with **1/15** the memory versus conventional methods, accurate up to **200 kHz**.
- **IMEX Solver for Nonlinear Components.** Splits PWL and nonlinear parts; uses **implicit** for PWL and **explicit** for nonlinear, removing the one-step delay via **two half-steps** to restore stability/accuracy. Verified on railway WPT at **75 ns** step.
- **X-in-the-Loop (XIL) with Stochastic Nonlinearity.** An FPGA **XIL testbench** integrates **polynomial chaos expansion** with a hybrid IMEX kernel to handle **stochastic** and **nonlinear** inductance; reaches **¼ the step size** of commercial testers with **½ the FPGA resources** on a 350-kW WPT (28 switches).

## Impact
- **Sub-µs, nanosecond-class timing.** End-to-end implementations at **12.5–75 ns** support converters at **200–400 kHz** with controller-consistent sampling and switch fidelity.
- **Stability without memory blow-up.** Implicit-level robustness using fixed MVM-centric iterations eliminates massive inverse tables, improving **scalability with switch count**.
- **Realistic environments.** Nonlinear magnetics and stochastic variations are supported **in real time**, enabling safer, broader controller validation than lab prototypes alone.
- **Sampling accuracy at fixed steps.** Half-step sampling doubles effective sampling rate without shrinking the integration step—capturing PWM edges and reducing duty bias.


## Publications

{{< cite page="/publication/zheng-semiimplicit-parallel-leapfrog-2023" view=1 >}}
{{< cite page="/publication/zheng-fpg-abased-real-time-xintheloop-2024" view=1 >}}
{{< cite page="/publication/zeng-real-time-digital-mapped-2024" view=1 >}}
{{< cite page="/publication/xu-topology-aware-matrix-partitioning-2023" view=1 >}}
{{< cite page="/publication/xu-fpga-based-implicit-explicit-realtime-2023" view=1 >}}



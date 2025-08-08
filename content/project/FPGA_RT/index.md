---
title: "Large-Scale Cyber-Physical System Co-Simulation"
summary: "Event-axis, synchronization-aware co-simulation that scales CHIL/PCCO from kW MMCs to MW-level converters by key-frame prediction, event-driven data rematching, and hybrid CPU–FPGA execution—boosting fidelity and easing real-time constraints."


tags:
  - Modeling
  - Sim
  - CPS
date: 2022-01-01
---
{{< youtube ijgKofb23cA >}}

## Overview
This project establishes a **large-scale cyber-physical co-simulation** stack for power electronics that unifies software simulators and **physical controllers**. We move from time-synchronous fixed-step interfaces toward **event-axis synchronization**, so the simulator–controller pair coordinates on switching and sampling events rather than rigid time ticks. The result is a system that **retains switching detail**, scales to **MW-level** plants, and remains robust under high data-interaction rates.


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
- **Scale & real-time tension.** Classical CHIL ties simulation step sizes to tight real-time budgets; as switching frequencies and device counts grow, maintaining fidelity forces costly hardware or model simplifications that distort dynamics. :contentReference[oaicite:0]{index=0} :contentReference[oaicite:1]{index=1}  
- **Interface bottlenecks.** Fixed-step synchronization (FSI) either wastes cycles or misses abrupt state changes; frequent handshakes balloon overhead and destabilize convergence in hybrid PES. :contentReference[oaicite:2]{index=2}  
- **Controller realism.** SIL/PIL miss hardware behaviors (ADC/PWM, multi-stage latency). We need a path that preserves **controller behavior consistency** without hard real-time. :contentReference[oaicite:3]{index=3}

## New Measures
- **Event-axis synchronization (ES-CHIL / EDS / ESTA).** Replace time-locked interaction with **event-synchronous** data exchange; use **state/switch events** to trigger both simulation and control computations, preserving logic while relaxing real-time constraints. :contentReference[oaicite:4]{index=4} :contentReference[oaicite:5]{index=5}  
- **Key-frame prediction + Adaptive Synchronization Interface (ASI).** Predict imminent state-change “key-frames” to **minimize synchronization points** and dynamically size steps across tools (e.g., Simulink ↔ DSIM). :contentReference[oaicite:6]{index=6}  
- **Self-restoring fault-tolerant data rematching.** A lightweight peripheral-IO strategy that **rematches control and simulation data** after link delays/failures—no simulator core changes—stabilizing high-rate controller–CPU co-simulation. :contentReference[oaicite:7]{index=7}  
- **Hybrid CPU–FPGA PCCO for MW-scale plants.** A **physical-controller co-simulation** (PCCO) architecture with event-driven sync executes detailed models (incl. switching) on CPU/FPGA while maintaining **controller behavior equivalence** to real systems. :contentReference[oaicite:8]{index=8}  
- **DSED-based plant models for loss/fidelity studies.** Use **discrete-state event-driven** simulation to evaluate losses and switching detail in **multi-terminal MW PETs** without exhaustive experiments. :contentReference[oaicite:9]{index=9}

## Impact
- **orders-of-magnitude sync efficiency.** ASI reduces synchronization time cost by **~394×** versus fixed-step interfaces while keeping accuracy in a 10-kVA MMC case. :contentReference[oaicite:10]{index=10}  
- **From kW MMCs to MW PETs.** Event-driven PCCO demonstrates a **2-MW PET with 576 switches** on a hybrid CPU–FPGA platform with preserved controller logic, expanding CHIL-class testing to MW-level systems. :contentReference[oaicite:11]{index=11}  
- **Robustness on commodity hardware.** The self-restoring method maintains accuracy under **high data-interaction frequencies** on **CPU-based simulators**, avoiding OS/kernel modifications. :contentReference[oaicite:12]{index=12}  
- **Higher-fidelity device phenomena.** Event-axis frameworks enable variable-step solvers and **natural commutation detection** (eliminating diode chattering), improving fidelity over time-locked CHIL. :contentReference[oaicite:13]{index=13}


## Publications

{{< cite page="/publication/zeng-self-restoring-fault-tolerant-method-2023" view=1 >}}
{{< cite page="/publication/zeng-event-synchronous-time-asynchronous-method-2023" view=1 >}}
{{< cite page="/publication/zheng-event-driven-synchronization-2024" view=1 >}}
{{< cite page="/publication/zheng-discrete-state-event-2020-a" view=1 >}}
{{< cite page="/publication/liu-adaptive-synchronization-interface-2024" view=1 >}}



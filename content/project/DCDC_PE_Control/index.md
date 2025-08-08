---
title: "Design and Control of High-Frequency DC–DC Converters"
summary: "From multi-DOF modulation and universal phase-shift control to device-aware electro-thermal modeling and CDT-MPC, this project delivers efficient, soft-switching, and control-ready designs for DAB/MMAB at 50–400 kHz+."


tags:
  - Modeling
  - Control
  - Edge
date: 2023-01-01
---

{{< youtube fGfJ54j6aaI >}}

## Overview
This project builds an end-to-end methodology for **high-frequency isolated DC–DC converters**—from **Dual/Multiactive Bridges (DAB/MMAB)** modulation to **device-aware models** and **control integration**. We systematize **multi-degree-of-freedom (M-DOF)** modulation for DAB, generalize it to MMAB via a **Universal Phase-Shift (UPS)** scheme, incorporate **SiC device electro-thermal transients** into design, and close the loop with **Cognitive Digital Twin–MPC (CDT-MPC)** for sensor-lean, high-performance control.

## Just Ask for questions！

Explore our research with an AI assistant powered by the latest Gemini models and reliable sources to enhance your understanding and analysis.

<div style="text-align:center; margin: 1rem 0;">
  <a href="https://notebooklm.google.com/notebook/b3d94d72-fdcf-4f2a-91d4-db61301d8501"
     class="btn btn-primary btn-lg"
     target="_blank" rel="noopener">
    Start exploring
  </a>
</div>


## Why This Research
- **Wide-bandgap + high f<sub>s</sub>:** Operation at 100–400+ kHz stresses soft-switching across wide ratios and loads; classical **SPS/DPS** loses ZVS and inflates RMS current at off-nominal conditions.  
- **Multi-port coupling:** MMAB efficiency/control suffer from tightly coupled ports and exploding DOFs without a unifying, scalable scheme.  
- **Device nonidealities:** SiC MOSFET/SBD transients and self-heating materially shape losses and thermal design—often ignored in system-level models.  
- **Control integration:** High-frequency dynamics demand **global state visibility** without high-bandwidth sensors and with strict timing guarantees.

## New Measures
- **M-DOF Modulation Synthesis for DAB.** We connect EPS/DPS/TPS/AMT into a single M-DOF view, showing how **zero-level sequences** regulate steady-state performance and mapping up to **5 DOFs** for H-bridges—providing actionable guidance for soft-switching and loss reduction.  
- **UPS for MMAB (Generalized Multi-Port).** A **Universal Phase-Shift** scheme yields a **time-domain model** and a **simple, scalable optimization** that achieves **full ZVS** and **minimized RMS inductor current** across port counts—validated on a **four-port prototype**.  
- **Mechanism-Segmentation Transient (MST) Model for SiC.** A **multi-rate electro-thermal** approach segments the **physical switching mechanisms** of SiC MOSFET/SBD, enabling fast, datasheet-driven loss/temperature prediction for converter-level design.  
- **CDT-MPC for HF Converters.** A **mode-driven numerical solver** plus **online parameter identification** forms a cognitive DT that feeds **MPC** with delay-free global states, delivering **dead-beat-like transients** without extra high-bandwidth sensors.

## Impact
- **Efficiency & Soft-Switching:** Restores **full ZVS** over wide operating regions and **reduces RMS currents**, improving conversion efficiency and thermal margins.  
- **Scalability:** UPS turns a multi-DOF problem into a **single-DOF optimization** that scales with port number and hardware complexity.  
- **Device-aware Design:** MST-based electro-thermal modeling shrinks the gap between simulation and hardware, guiding magnetics/thermal sizing and reliability.  
- **Control Performance:** CDT-MPC integrates complete-model predictions **in real time**, cutting sensor latency and improving dynamic response and robustness.


## Publications

{{< cite page="/publication/zheng-cognitive-digital-twins-based-2025" view=1 >}}
{{< cite page="/publication/mou-overview-multi-degreeof-freedom-modulation-2023-a" view=1 >}}
{{< cite page="/publication/wang-universal-phase-shift-modulation-2024-a" view=1 >}}




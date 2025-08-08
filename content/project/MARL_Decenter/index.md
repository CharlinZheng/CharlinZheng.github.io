---
title: "SNA: A Network-Aware Framework for Decentralized Inverter-Based Voltage Control"
summary: "Network-aware multi-agent RL that scales decentralized secondary voltage control by truncating critics to κ-hop neighborhoods with provable approximation guarantees; validated up to 114 DGs."
tags:
  - ML
  - Grid
date: 2022-01-01
---

{{< youtube kUE9RBzCgLk >}}

## Overview

This project develops a **Scalable Network-Aware (SNA)** learning framework for **decentralized secondary voltage control** in inverter-dominated distribution grids. Instead of relying on centralized critics that ingest global states/actions, SNA leverages the **grid’s network structure** so each critic only depends on **local and κ-hop neighbor** information, while actors are guided by their neighbors’ critics. This respects physical coupling, reduces input dimensionality, and preserves cooperation—enabling practical learning-based voltage regulation in large systems.

## Why This Research

* **Operational pressure is rising.** Variable renewables and prosumers cause fast, uncertain power fluctuations that defeat traditional capacitor/regulator-based schemes and leave **primary droop control** with steady-state voltage deviations. Decentralized **secondary** control is needed to restore nominal voltages at scale.
* **Dominant MARL training is not scalable.** Centralized Training & Decentralized Execution (CTDE) makes each critic depend on **global** observations/actions; dimension grows with the number of agents, causing sample inefficiency and poor training in large grids.
* **Untapped prior: grid topology.** Voltage control naturally has **local interactions** on the network. If we exploit this locality, we can cut critic inputs without losing the signal actors need to cooperate.
* **Goal.** Achieve **scalable, theoretically justified** decentralized voltage control that keeps voltages within limits under stochastic loads and model imperfections, while requiring only **neighbor-level** information exchange during training.

## New Measures

* **Networked-MDP formulation of voltage control.** The grid is modeled so that a DG’s next-state distribution depends only on its neighbors, aligning with EMTP-style discretization where interactions are effectively local.
* **Exponential-decay property ⇒ truncated critics.** We prove that an agent’s Q-function sensitivity to distant nodes **decays exponentially** with graph distance; hence a critic that only sees **κ-hop** observations/actions approximates the true Q with a bounded error $\le c \rho^{\kappa+1}$.
* **Distributed actor guidance.** Each actor is updated using the **sum of its neighbors’ truncated critics**, promoting local cooperation that aligns with global welfare—without any global critic.
* **Algorithm-agnostic integration.** SNA plugs into standard multi-agent actor-critic methods (e.g., **MASAC**, **MATD3**) by replacing the critic inputs and actor objectives accordingly.
* **Communication-efficient training.** Training requires only **neighbor exchanges** (tunable by κ), reducing bandwidth and improving privacy, with κ=1 often sufficient in practice.

## Impact

* **Scalability from tens to 100+ DGs.** SNA trains effectively on systems with **up to 114 DGs**, surpassing prior decentralized voltage-control studies limited to ≈40 agents.
* **Better training performance at scale.** Compared to CTDE baselines, SNA attains **higher final training rewards** as agent count grows (e.g., 84/114 DGs), evidencing improved sample efficiency and critic learnability.
* **Voltage quality improvements.** Under identical disturbances, SNA **reduces voltage-magnitude excursions** versus PI and CTDE-trained policies; the proportion of nodes exceeding ±0.05 pu shrinks notably in large cases.
* **Tunable locality for accuracy vs. complexity.** Increasing κ tightens the approximation but enlarges inputs; on 114-DG systems, **κ=2** can improve rewards, while **κ=3** may hurt due to dimensionality—guiding practical κ selection.
* **Plug-and-play across algorithms.** Integrating SNA with **MATD3** similarly boosts final rewards, showing method generality beyond MASAC.
* **Deployment-friendly.** Because SNA relies on neighbor-level data and distributed training, it aligns with **realistic utility communications**, easing field integration.

## Publications

{{< cite page="/publication/xu-scalable-network-aware-multi-agent-2023" view="Stream" >}}





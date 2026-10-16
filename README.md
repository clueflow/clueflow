<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)"
            srcset="assets/clueflow-logo-light.png">
    <source media="(prefers-color-scheme: light)"
            srcset="assets/clueflow-logo-dark.png">
    <img src="assets/clueflow-logo-dark.png"
         alt="ClueFlow"
         width="480">
  </picture>
</div>

<p align="center">
  <strong>Learning Long-Horizon Search through Attributed Research-State Transitions</strong>
</p>

## Overview

**ClueFlow** is a stateful search agent harness that provides a unified research-state interface for **long-horizon inference, trajectory generation, and post-training**.

At inference time, ClueFlow equips language models with browser tools and persistent **Evidence** and **Candidate** states. Agents can accumulate evidence, track competing hypotheses, and revise their research states across extended interactions while operating with bounded context windows.

The same stateful execution interface supports teacher trajectory collection and online reinforcement learning rollouts. ClueFlow records browser actions and structured state transitions, enabling **Source–State–Final attribution** that connects information acquisition, validated research progress, and final-answer decisions.

These attributed transitions provide a shared foundation for **SFT data construction and reinforcement learning credit assignment**, including the recovery of useful intermediate progress from unsuccessful trajectories.

<p align="center">
  <a href="assets/clueflow-method-overview.pdf">
    <img src="assets/clueflow-method-overview.png"
         alt="ClueFlow method overview: stateful trajectory generation, Source–State–Final attribution, attribution-guided SFT, and Turn-PPO"
         width="100%">
  </a>
</p>

## Core Capabilities

**Stateful Search Inference.** Execute long-horizon search with persistent research states, structured tool operations, and bounded interaction histories.

**Trajectory Generation.** Collect reproducible search trajectories with browser observations, state transitions, and action provenance.

**Transition Attribution.** Validate Evidence and Candidate updates and trace supported research progress back to the browser actions that produced it.

**Post-Training Support.** Construct attribution-guided SFT examples and turn-level credit signals for PPO using a shared trajectory representation.

## Release Status

The ClueFlow source code, documentation, and research artifacts will be released soon. Please stay tuned for updates.

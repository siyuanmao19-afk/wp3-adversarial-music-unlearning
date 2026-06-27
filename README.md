# WP3 Adversarial Music Unlearning

This repository is for WP3: **Music Unlearning in Feature Space**.

The project investigates a GAN-inspired adversarial unlearning framework for generative music models. The goal is to suppress a target musical concept, such as a style or artist-like signature, while preserving general music generation quality.

## Research Question

Can a GAN-inspired adversarial unlearning method suppress a target musical style in a generative music model while preserving general music generation ability?

## Core Idea

1. Train a target-style discriminator to detect the music concept that should be forgotten.
2. Adapt the generator so that generated outputs receive lower target-style probability.
3. Use retain/preservation losses and audio quality metrics to reduce collateral damage.

## Team Roles

- Member A: baseline model, generation scripts, generator adaptation.
- Member B: forget/retain datasets, target-style discriminator, evaluation metrics.
- Member C: experiment protocol, logging, baseline comparison, result tables, paper structure.

## Repository Structure

```text
wp3-adversarial-music-unlearning/
  data/
    forget_set/
    retain_set/
    metadata/
  scripts/
  configs/
  outputs/
    audio_before/
    audio_after/
    checkpoints/
    results/
    logs/
  paper/
    figures/
    tables/
  docs/
```

## Important

Large files such as audio samples, model checkpoints, and generated datasets should not be committed directly to GitHub. Use shared storage or Git LFS if needed.


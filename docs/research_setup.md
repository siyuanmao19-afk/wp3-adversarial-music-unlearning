# WP3 Research Setup

## Project Title

GAN-Inspired Adversarial Music Unlearning in Feature Space

## Research Question

Can a GAN-inspired adversarial unlearning method suppress a target musical style in a generative music model while preserving general music generation ability?

## Motivation

Pre-trained music generation models may learn protected or unwanted musical styles from large-scale datasets. Retraining the full model from scratch is expensive. WP3 investigates whether post-training adversarial unlearning can reduce the model's ability to generate a target musical concept while maintaining general generation quality.

## Target Concept

- Target style: TBD
- Reason for choosing this target: TBD
- Forget set source: TBD
- Retain set source: TBD

## Baseline Model

- Model name: TBD
- Model version: TBD
- Local machine / environment: TBD
- Input prompt format: TBD
- Output audio format: TBD

## Main Method

We use a GAN-inspired adversarial unlearning framework:

1. Train a target-style discriminator to detect the target musical concept.
2. Adapt the generator so that its outputs receive lower target-style probability from the discriminator.
3. Add retain/preservation loss to reduce collateral damage on non-target prompts.

## Evaluation Questions

1. Forgetting success: does target-style similarity decrease after unlearning?
2. Utility preservation: does the model still generate non-target music well?
3. Audio quality: does unlearning introduce artifacts or reduce fidelity?

## Planned Metrics

- Target-style discriminator score: TBD
- CLAP / prompt alignment: TBD
- FAD or alternative audio quality metric: TBD
- Human listening notes: TBD


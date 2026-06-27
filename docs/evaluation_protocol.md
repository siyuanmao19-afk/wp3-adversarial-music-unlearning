# WP3 Evaluation Protocol

## Evaluation Goal

Evaluate whether adversarial unlearning successfully reduces target-style generation while preserving general music generation quality.

## Conditions to Compare

At minimum:

1. Original model
2. Adversarial unlearning model
3. One baseline method

## Metrics

### Forgetting Success

- Target-style discriminator probability
- Target-style similarity reduction

### Utility Preservation

- CLAP / prompt alignment score
- Retain prompt performance

### Audio Quality

- FAD or alternative quality metric
- Human quality score
- Artifact notes

## Main Tables

- Table 1: Original vs unlearned model.
- Table 2: Adversarial unlearning vs baseline method.
- Table 3: Ablation study on loss weights or model update scope.


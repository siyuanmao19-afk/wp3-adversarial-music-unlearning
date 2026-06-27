# Target-Style Discriminator Protocol

## Purpose

The target-style discriminator is trained to identify whether an audio sample belongs to the target musical concept. It will be used both for evaluation and as the adversarial signal in unlearning.

## Target Style

- Target style: TBD
- Definition: TBD
- Positive examples source: TBD
- Negative examples source: TBD

## Dataset Split

- Forget set version: TBD
- Retain set version: TBD
- Train split: TBD
- Validation split: TBD
- Test split: TBD

## Input Representation

Choose one:

- Raw audio
- Mel-spectrogram
- CLAP embedding
- Other audio embedding

## Required Output Format

Each evaluated audio sample should produce:

```json
{
  "audio_id": "",
  "target_style": "",
  "target_probability": 0.0,
  "predicted_label": "",
  "model_checkpoint": ""
}
```


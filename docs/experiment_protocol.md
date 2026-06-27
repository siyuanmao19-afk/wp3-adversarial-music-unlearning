# WP3 Experiment Protocol

## Experiment Naming Rule

Use:

```text
model_method_target_date_seed
```

Example:

```text
musicgen_advunlearn_jazzpiano_20260701_seed1
```

## Audio Naming Rule

Use:

```text
experimentid_promptid_seed.wav
```

Example:

```text
musicgen_baseline_jazzpiano_20260701_seed1_t001.wav
```

## Prompt Types

- `target`: prompts directly related to the target style.
- `retain`: prompts related to non-target styles that should be preserved.
- `general`: broad music prompts.
- `ambiguous`: prompts that may partially overlap with the target.

## Required Metadata for Each Audio File

- audio_id
- experiment_id
- model
- method
- target_style
- prompt_type
- prompt_id
- prompt_text
- seed
- date
- generated_by
- audio_path

## Minimum Week 3 Baseline Plan

- Target prompts: 10
- Retain prompts: 10
- Seeds per prompt: 2
- Total generated audio: 40


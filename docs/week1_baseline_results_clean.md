# Week 1 Baseline Results

## Summary

I reproduced the baseline inference pipeline for `facebook/musicgen-small` using Hugging Face Transformers. The model was run locally with CUDA on an NVIDIA RTX 4070 Laptop GPU.

## Model

| Item | Value |
|---|---|
| Model | `facebook/musicgen-small` |
| Task | Text-to-music generation |
| Output format | WAV |
| Sample rate | 32000 Hz |

## Environment

| Item | Value |
|---|---|
| OS | Windows |
| GPU | NVIDIA GeForce RTX 4070 Laptop GPU |
| Driver | 566.07 |
| CUDA shown by `nvidia-smi` | 12.7 |
| GPU memory | 8188 MiB |
| Device used | CUDA |

## Generated Baseline Samples

| File | Prompt | Duration |
|---|---|---:|
| `outputs/jazz.wav` | `A relaxing jazz piano solo with soft drums` | ~5s |
| `outputs/rock.wav` | `An energetic rock guitar solo with powerful drums` | ~5s |
| `outputs/edm.wav` | `Electronic dance music with a strong beat and synth bass` | ~5s |
| `outputs/classical.wav` | `A classical orchestra with violin cello and piano` | ~5s |

## Runtime

One end-to-end test was measured with PowerShell `Measure-Command`.

| Item | Value |
|---|---:|
| Output file | `outputs/time_test.wav` |
| Prompt | `A calm piano melody with soft strings` |
| Audio duration | ~5s |
| Total runtime | 25.30s |

The measured runtime includes script launch, environment setup, model loading, audio generation, and WAV saving.

## Notes

- The model successfully ran on CUDA.
- The generated files were saved under `outputs/`.
- Hugging Face authentication warning appeared, but it did not block inference.
- Transformers configuration warnings appeared, but the model still loaded and generated audio successfully.

## Status

Week 1 baseline reproduction is complete. The next step is to support batch generation and metadata logging for a larger prompt set.

# CUE Meets LRP

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vincent-el/cue-meets-lrp/blob/main/cue_meets_lrp.ipynb)

Exploring how different LRP composite rules explain the same prediction, evaluated through the [CUE model](https://arxiv.org/abs/2506.14775) lens (Labarta et al., 2025).

## What it does

1. Loads VGG16 and classifies one image
2. Applies three [zennit](https://github.com/chr5tphr/zennit) composite rules to produce heatmaps
3. Scores each on CUE dimensions (Legibility, Readability, Interpretability) using simple proxies
4. Asks BLIP-2 (VLM) for a second perspective on each explanation

## Run locally

```bash
pip install zennit torchvision transformers accelerate
jupyter notebook cue_meets_lrp.ipynb
```

Or click the Colab badge above for zero-setup execution.

*Vincent Lange · vincentelange@gmail.com*

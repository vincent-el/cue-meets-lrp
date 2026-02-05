# CUE Meets LRP

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vincent-el/cue-meets-lrp/blob/main/cue_meets_lrp.ipynb)

Applying three LRP composite rules via [zennit](https://github.com/chr5tphr/zennit) and evaluating explanation quality through the [CUE model](https://arxiv.org/abs/2506.14775) lens (Labarta et al., 2025).

## What it does

- Loads VGG16 and classifies three sample images (animal, scene, object)
- Applies three zennit composite rules to produce 9 heatmaps
- Scores each heatmap on CUE dimensions (Legibility, Readability, Interpretability) using perceptual proxies
- Runs a small VLM (moondream2) for a "cognitive" second opinion on each explanation

## Run locally

```bash
pip install zennit torchvision
jupyter notebook cue_meets_lrp.ipynb
```

Or click the Colab badge above for zero-setup execution with free GPU.

*Vincent Lange · vincentelange@gmail.com*

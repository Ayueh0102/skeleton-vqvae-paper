# Discrete Representation Learning for Chinese Calligraphy Skeletons

**From Distance Fields to Conditional Generation**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Railway-blueviolet)](https://skeleton-vqvae-paper-production.up.railway.app)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

---

## Overview

A systematic study of discrete representation learning for Chinese calligraphy character skeletons, spanning **20 experimental phases** across 6 tokenizer architectures and 4 generation methods on **20,000 characters** at 128×128 resolution.

### Key Results

| Metric | Value |
|--------|:-----:|
| Reconstruction IoU | **0.994** |
| Cross-font generalization (7 fonts incl. cursive) | **IoU > 0.988** |
| Stroke count prediction (R²) | **0.833** |
| IDS structure classification | **80.0%** |
| Generation connectivity (Hierarchical MaskGIT) | **98.6%** |
| Generation NN IoU | **0.875** |

### Highlights

- **Distance field input** transforms sparse skeleton (3% pixels) into dense signal → +12pt IoU
- **EMA VQ-VAE 256 tokens** matches continuous baseline with zero discretization cost
- **Cross-font transfer** works even on cursive/grass script (max drop 0.57pt)
- **Hierarchical MaskGIT** (coarse 16 + fine 256 tokens) achieves 98.6% structural connectivity
- **7 negative results** systematically documented with root cause analysis

## Authors

- **Chun-Ting Yueh (岳俊廷)** — Independent Researcher
- **Claude Opus 4.6** — AI Co-Author (Anthropic)
- **GPT-5.4 xHigh** — AI Co-Author (OpenAI)

## Live Paper

**[https://skeleton-vqvae-paper-production.up.railway.app](https://skeleton-vqvae-paper-production.up.railway.app)**

Features:
- Full bilingual paper (EN/ZH toggle)
- 12 tables + 20+ figures
- Interactive image zoom
- Glossary of 17 key concepts
- Design decisions: expectations vs. reality (Table 9)

## Repository Structure

```
├── index.html          # Main paper page (self-contained HTML)
├── paper/
│   └── figures/        # QR codes and supplementary images
├── viewer/             # All experiment result figures (67 PNGs)
└── package.json        # Railway deployment config
```

## Citation

```
@misc{yueh2026skeleton,
  title={Discrete Representation Learning for Chinese Calligraphy Skeletons: 
         From Distance Fields to Conditional Generation},
  author={Yueh, Chun-Ting},
  year={2026},
  url={https://skeleton-vqvae-paper-production.up.railway.app}
}
```

## License

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

## Contact

- Email: yueh3321387@gmail.com
- LinkedIn: [chun-ting-yueh](https://www.linkedin.com/in/chun-ting-yueh)

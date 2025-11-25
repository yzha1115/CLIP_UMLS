# Medical Image-Text Retrieval with Knowledge Enhancement

Research code for our IEEE ISBI 2026 submission on zero-shot medical image-text retrieval.

## Status

Paper under review. Full code will be released upon acceptance.

## Overview

This work enhances medical image-text retrieval through structured medical knowledge integration. We evaluate on the ROCO dataset using BiomedCLIP as the base model.

## Dataset

ROCO (Radiology Objects in COntext): 81,825 medical images with captions

Dataset available at: https://huggingface.co/datasets/rvl-lab/roco

## Results

Performance on ROCO test set (8,183 image-text pairs):

| Method | R@1 | R@5 | R@10 | MedR |
|--------|-----|-----|------|------|
| BiomedCLIP Baseline | 79.27% | 96.17% | 98.35% | 1 |
| Our Approach | 93.04% | 97.85% | 98.35% | 1 |

![Retrieval Results](results/retrieval_comparison.png)

## Repository Contents

Currently available:
- Baseline evaluation code (`baseline/`)
- Requirements and dependencies
- Results visualization

Complete implementation will be released after paper acceptance.

## Installation

```bash
git clone https://github.com/yzha1115/CLIP_UMLS.git
cd CLIP_UMLS
pip install -r requirements.txt
```

## Usage

Run baseline evaluation:
```bash
jupyter notebook baseline/biomedclip_baseline.ipynb
```

## Citation

```bibtex
@inproceedings{ye2026medical,
  title={Enhancing Medical Image-Text Retrieval Through UMLS Metadata Integration},
  author={Ye, Zhang Chee Ming and Ting, Chee-Ming and others},
  booktitle={IEEE ISBI},
  year={2026}
}
```

## Contact

Ye Zhang
yzha1115@student.monash.edu
zhangye0624@gmail.com

## Acknowledgments

This work uses BiomedCLIP (Microsoft Research) and the ROCO dataset.

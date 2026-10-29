<h1 align="center">BiCoDA</h1>

<p align="center">
  <strong>A Bidirectional Cooperative Defect Analysis Model for Wafer Die Defect Detection and Semantic Segmentation</strong>
</p>

---

## Overview

Wafer die defects vary in scale, texture, and morphology. Bounding boxes may not adequately represent irregular defect boundaries, while segmentation alone does not provide object-level localization.

**BiCoDA** jointly addresses these challenges through a shared encoder and bidirectional information exchange between detection and segmentation branches. It integrates spatial, frequency-domain, and edge features. Segmentation masks also guide detection-box refinement during inference.

## Results

Results on the **Wafer-Defect-rv1vx** dataset:

| Metric | Result |
|:--|--:|
| mAP@0.5 | 78.72% |
| mAP@0.5:0.95 | 52.84% |
| Dice | 82.32% |
| IoU | 72.32% |
| Parameters | 42.71M |
| Inference speed | 86 FPS |

## Requirements

- Ubuntu 24.04
- Python 3.10
- CUDA 13.0
- PyTorch 2.12.1

## Installation

Create and activate the Conda environment:

```bash
conda env create --name bicoda --file environment.yml
conda activate bicoda

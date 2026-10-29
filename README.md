# BiCoDA

## A Bidirectional Cooperative Defect Analysis Model for Wafer Die Defect Detection and Semantic Segmentation

BiCoDA is a unified framework for wafer die defect detection and semantic segmentation. Wafer defects vary substantially in scale, texture, and morphology. Bounding boxes can be insufficient to represent irregular defect boundaries, while semantic segmentation alone does not provide reliable object-level classification and localization.

BiCoDA addresses these complementary challenges through a shared feature encoder and bidirectional cooperation between its detection and segmentation branches. The model integrates spatial, frequency-domain, and edge representations. Segmentation features provide region and boundary cues to improve detection, while detection predictions provide class and location context to guide segmentation. During inference, predicted masks support geometric refinement of detection boxes.

## Key Results

Evaluated on the Wafer-Defect-rv1vx dataset, BiCoDA achieves:

| Metric | Result |
|---|---:|
| mAP@0.5 | 78.72% |
| mAP@0.5:0.95 | 52.84% |
| Dice | 82.32% |
| IoU | 72.32% |
| Parameters | 42.71M |
| Inference speed | 86 FPS |

## Method Overview

- **Shared feature encoding:** Combines spatial, frequency-domain, and edge representations.
- **Bidirectional cooperation:** Exchanges complementary information between detection and segmentation.
- **Mask-guided localization:** Uses predicted masks to refine detection-box geometry during inference.
- **Joint prediction:** Supports defect classification, object-level localization, and pixel-level delineation in one framework.

## Code Availability

The source code for this study will be made publicly available at:

[https://github.com/Heyue991208/BiCoDA](https://github.com/Heyue991208/BiCoDA)

## Citation

Citation details will be added when the publication information is available.

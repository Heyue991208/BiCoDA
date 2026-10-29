# BiCoDA
BiCoDA: A Bidirectional Cooperative Defect Analysis Model for Wafer Die Defect Detection and Semantic Segmentation

Wafer die defects vary widely in scale, texture, and morphology, making bounding boxes insufficient for describing irregular boundaries and segmentation alone inadequate for object-level localization. We propose BiCoDA, a unified model for defect detection and semantic segmentation. It uses a shared encoder with spatial, frequency-domain, and edge features, and enables bidirectional information exchange between detection and segmentation branches. Mask-guided box refinement further improves localization. On the Wafer-Defect-rv1vx dataset, BiCoDA achieves 78.72% mAP50, 52.84% mAP50-95, 82.32% Dice, and 72.32% IoU, with 42.71 million parameters and an inference speed of 86 FPS. 

The project code will be open-sourced soon.

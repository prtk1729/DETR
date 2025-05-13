
# DETR - End-to-End Object Detection with Transformers

This project implements DETR (DEtection TRansformer), a novel transformer-based object detection model introduced by Facebook AI. Unlike traditional object detectors, DETR eliminates the need for anchor boxes and non-maximum suppression (NMS), reframing object detection as a direct set partition problem.

## 🔍 Key Highlights

- End-to-end object detection using transformer architecture
- Anchor-free and NMS-free detection
- Hungarian bipartite matching for one-to-one prediction alignment
- DETR architecture breakdown: CNN backbone + transformer encoder-decoder + object queries
- Custom loss function combining classification and bounding box regression

## 🏗️ Architecture Overview

- **Backbone:** CNN (e.g., ResNet-50) for feature extraction
- **Transformer Encoder-Decoder:** Encodes spatial features and decodes them using learned object queries
- **Set Prediction:** Predicts fixed-size set of boxes and labels using bipartite matching
- **Loss Function:** Combines cross-entropy loss and L1/GIoU loss using Hungarian matching

## 📦 Upcoming

In the next phase, the model will be trained and evaluated on the PASCAL VOC dataset using the architecture and loss formulations explored here.

## 📚 References

- [End-to-End Object Detection with Transformers (DETR)](https://arxiv.org/abs/2005.12872) — Facebook AI


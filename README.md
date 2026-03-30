# NANOMIND Code

## Intro

NANOMIND is a multimodal on-device inference framework for small, battery-powered systems.

The project focuses on a software-hardware co-design approach for running multimodal AI workloads efficiently on resource-constrained edge devices. Instead of treating the full stack as a monolithic model invocation, NANOMIND is built around modular execution, heterogeneous accelerator usage, and low-power runtime design.

## Background

Modern multimodal systems are increasingly expected to run directly on edge devices for privacy, responsiveness, and offline operation. In practice, however, small devices are constrained by power, memory, and heterogeneous hardware limits.

NANOMIND explores a practical system design for this setting:

- modular multimodal inference,
- cross-accelerator scheduling,
- unified-memory-aware execution,
- hardware-software co-design,
- low-power and battery-aware deployment.

## Paper

- **Tiny but Mighty: A Software-Hardware Co-Design Approach for Efficient Multimodal Inference on Battery-Powered Small Devices**
- Published at **ICLR 2026**
- Local PDF: [`tinyLLM.pdf`](./tinyLLM.pdf)
- Public paper/project link: **to be added**

## Repository Status

This repository is **still being organized for public release**.

It is not yet the full open-source release of the internal research codebase. The current goal of this public repository is to:

1. provide the paper and project context,
2. publish the model assets and reusable components that can be shared cleanly,
3. gradually build toward a proper public-facing code release.

The private development repository and the public GitHub repository are intentionally kept separate.

## Current Public Contents

At the moment, this repository contains:

- [`tinyLLM.pdf`](./tinyLLM.pdf): the paper,
- [`models/`](./models): model assets that are currently ready to share publicly.

More code, documentation, and reproducible components will be added as the repository is cleaned up.

## Models

The [`models/`](./models) directory currently includes selected runtime model assets used by the `Nanomind_Virgile` stack:

- `models/yolo/yolo11n_int8.rknn`
- `models/clip/clip_images.rknn`
- `models/clip/clip_text.rknn`
- `models/insightface/scrfd_2.5g_bnkps_renamed.onnx`
- `models/insightface/r18_glint360k.onnx`
- `models/insightface/Gundam_RK356X.tar.gz`

These are included as reference/runtime assets for the current public snapshot.

### Model Status Notes

- **YOLO / CLIP / InsightFace runtime assets**: included in this public snapshot.
- **LLM base model assets**: still being organized for public release.
- **Qwen-related base model packaging**: not published here yet.

## Intended Direction

This repository will eventually focus on the publicly shareable parts of the NANOMIND system, including:

- edge multimodal inference building blocks,
- deployment-oriented runtime components,
- selected model packaging,
- documentation for reproducing core ideas from the paper.

## Disclaimer

This repository is still under construction.

Interfaces, directory structure, included assets, and documentation may change as the public release is assembled.

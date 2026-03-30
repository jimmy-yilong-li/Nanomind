# Models

This folder stores the model assets that are currently safe and ready to include in the public repository.

## Included now

### YOLO

- `yolo/yolo11n_int8.rknn`
  - RKNN runtime weight used for lightweight object detection on RK3566

### CLIP

- `clip/clip_images.rknn`
  - CLIP image encoder runtime weight
- `clip/clip_text.rknn`
  - CLIP text encoder runtime weight

### InsightFace / InspireFace

- `insightface/scrfd_2.5g_bnkps_renamed.onnx`
  - compact SCRFD face detector model
- `insightface/r18_glint360k.onnx`
  - ArcFace-style face embedding model
- `insightface/Gundam_RK356X.tar.gz`
  - InspireFace RK356X pack archive

## Still being organized

- The LLM base model assets, including the Qwen-related part of the stack, are still being organized for public release.
- Some runtime naming and packaging in the private deployment differ from what will eventually be published here.

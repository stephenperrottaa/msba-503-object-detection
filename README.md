#MSBA 503 Take Home Assignment

#Overview
- Compare two pretrained COCO detectors on 10 images in `data/images`:
  - YOLOv8n (Ultralytics) — single-stage, speed-focused.
  - Faster R-CNN ResNet50 FPN (torchvision) — two-stage, higher recall.
- Confidence threshold: 0.25 for both.
- Outputs: `outputs/detection_comparison.csv` (per-image timing/detections) and `outputs/image_color_stats.csv` (non-DL stats).

#Files
- `take_home_assignment_final.ipynb`: main notebook with code and printed outputs.
- `outputs/detection_comparison.csv`: comparison table (image, model, inference time, objects detected, top predictions).
- `outputs/image_color_stats.csv`: size and mean color/brightness stats.
- `yolov8n.pt`: YOLO weights (not needed if Ultralytics downloads automatically; add to `.gitignore` if keeping local).

#How to run
1) Install dependencies:
   ```bash
   pip install ultralytics torch torchvision matplotlib pandas pillow numpy

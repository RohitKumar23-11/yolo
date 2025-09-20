# YOLO Project

## Structure
```
yolo/
├─ notebooks/
│ └─ yolo_study_and_pipeline.py
├─ src/
│ ├─ augmentations.py
│ ├─ data_loader.py
│ ├─ train_yolo.py
│ ├─ video_baseline.py
│ └─ utils.py
├─ data/
│ └─ coco_dataset.yaml
└─ README.md
```

## Contents
- **notebooks/** → Jupytext-style notebook for running end-to-end experiments
- **src/** → Source code for augmentations, dataloading, training, video models, and utilities
- **data/** → Dataset YAML for YOLO training

## Usage
1. Install requirements:
```bash
pip install ultralytics albumentations matplotlib torch torchvision
```
2. Train YOLO:
```bash
python src/train_yolo.py
```
3. Run video classification baseline by importing `CNNLSTM`.

# Pretrained Weights

This directory is intended to store the pretrained model weights for **Vision Phoenix (VPH)**.

---

## Available Weights

At present, pretrained VPH weights are **not included** in this repository.

The pretrained models will be released after the associated manuscript has completed the peer-review and publication process.

---

## Baseline Weights

The Vision Phoenix (VPH) framework is implemented on top of **YOLOv7**.

Please download the official YOLOv7 pretrained weights from the official repository:

- Official YOLOv7 Repository: https://github.com/WongKinYiu/yolov7

Typical pretrained weights include:

```
yolov7.pt
yolov7x.pt
yolov7-tiny.pt
```

Place the downloaded weights in this directory before training or evaluation.

Example:

```
weights/
├── yolov7.pt
├── vph.pt          (released after publication)
└── README.md
```

---

## Training Your Own Model

You can reproduce the reported results by training Vision Phoenix (VPH) using the provided configuration files and scripts.

Example:

```bash
python train.py --workers 8 --device 0 --batch-size 16 --epochs 1 --img 640 640  --data data/V7_VPH.yaml --hyp data/hyp.scratch.custom.yaml --cfg cfg/training/yolov7_VPH_P4.yaml --name VPH --weights weights/yolov7.pt

```

---

## Future Updates

After publication, this directory will be updated with:

- Vision Phoenix (VPH) pretrained weights
- Performance checkpoints
- Model configuration files
- Inference examples
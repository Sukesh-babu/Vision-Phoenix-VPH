# Dataset Preparation

Vision Phoenix (VPH) is evaluated on multiple publicly available pedestrian detection datasets. Due to copyright and licensing restrictions, the datasets are **not distributed** with this repository. Please obtain them from their respective official sources and organize them as described below.

---

# Directory Structure

```
data/
│
├── COCO-Person/
├── WiderPerson/
├── CamPedV2/
├── CrowdHuman/
├── LLVIP/
├── RTTS/
├── FoggyCityscapes/
└── UCSD/
```

---

# Benchmark Datasets

## COCO-Person

- **Purpose:** Quantitative evaluation
- **Official Website:** https://cocodataset.org/

Use the official **train2017** and **val2017** splits.

---

## WiderPerson

- **Purpose:** Quantitative evaluation
- **Official Website:** http://www.widerperson.net/

Use the official training and validation splits.

---

## CamPedV2

- **Purpose:** Quantitative evaluation

CamPedV2 is a large-scale real-world pedestrian detection dataset developed for robust pedestrian detection under challenging environmental conditions, including adverse weather, occlusion, scale variation, and pedestrian-like distractors.

**Publication:**

> V. S. Sukesh Babu and Rahul Raman,  
> *CamPedV2: A Diverse Real-Time Pedestrian Detection Dataset for Challenging Environmental Conditions*,  
> **The Visual Computer**, vol. 42, no. 9, Article 351, 2026.  
> DOI: 10.1007/s00371-026-04566-z

**Official Article:**  
https://doi.org/10.1007/s00371-026-04566-z

**Official Dataset Repository:**  
:contentReference[oaicite:0]{index=0}

Please download the dataset from the official repository and place it under:

```text
data/
└── CamPedV2/
```

---

## CrowdHuman

- **Purpose:** Dense crowd evaluation
- **Official Website:** https://www.crowdhuman.org/

---

## LLVIP

- **Purpose:** Low-light qualitative evaluation
- **Official Website:** https://bupt-ai-cz.github.io/LLVIP/

---

## RTTS

- **Purpose:** Rainy and hazy scene evaluation

Available through the RESIDE benchmark:

https://sites.google.com/view/reside-dehaze-datasets

---

## Foggy Cityscapes

- **Purpose:** Foggy weather evaluation
- **Official Website:** https://www.cityscapes-dataset.com/

---

## UCSD Pedestrian Dataset

- **Purpose:** Pedestrian-like object evaluation
- **Official Website:** http://www.svcl.ucsd.edu/projects/anomaly/dataset.htm

---

# Dataset Configuration

Update the corresponding dataset YAML files in the `data/` or `cfg/` directory to match the local dataset paths.

---

# Experimental Protocol

- Official training, validation, and testing splits are used for all benchmark datasets.
- No overlap exists between training, validation, and testing subsets.
- Please comply with the respective dataset licenses before use.

---

# CamPedV2 Citation

If you use CamPedV2 in your research, please cite:

```bibtex
@article{sukesh2026campedv2,
  title={CamPedV2: A Diverse Real-Time Pedestrian Detection Dataset for Challenging Environmental Conditions},
  author={Sukesh Babu, V. S. and Raman, Rahul},
  journal={The Visual Computer},
  volume={42},
  number={9},
  pages={351},
  year={2026},
  doi={10.1007/s00371-026-04566-z}
}
```
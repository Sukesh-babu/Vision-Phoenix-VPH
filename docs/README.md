# Documentation

This directory contains the architecture figures used in the Vision Phoenix (VPH) repository and the accompanying manuscript.

---

## Files

### VPH_Overall.jpg

**Description**

Overall architecture of the proposed Vision Phoenix (VPH) framework.

The figure illustrates the integration of the VPH module into the P4 feature level of the YOLOv7 PAN-FPN neck. The refined feature representations are subsequently forwarded to the multi-scale detection head for pedestrian detection.

This figure corresponds to **Figure 1** in the manuscript.

---

### VPH_Internal.jpg

**Description**

Internal architecture of the proposed Vision Phoenix (VPH) module.

The module performs latent-state context reasoning through six sequential stages:

1. Tokenization
2. Latent Projection
3. Latent-State Interaction
4. Feature Reconstruction
5. Reshape
6. Residual Fusion

This figure corresponds to **Figure 2** in the manuscript.

---

## Vision Phoenix Pipeline

The proposed VPH framework operates as follows:

```
Input Feature Map
        │
        ▼
Tokenization
        │
        ▼
Latent Projection
        │
        ▼
Latent-State Interaction
        │
        ▼
Feature Reconstruction
        │
        ▼
Reshape
        │
        ▼
Residual Fusion
        │
        ▼
Output Feature Map
```

The module performs efficient context reasoning in a compact latent-state space while preserving computational efficiency through residual feature fusion.

---

## Citation

If you use these figures or the Vision Phoenix (VPH) framework in your research, please cite the associated publication.

```bibtex
@article{sukesh2026vph,
  title={Vision Phoenix: Efficient Latent-State Context Reasoning for Robust Pedestrian Detection},
  author={Sukesh Babu, V. S. and Raman, Rahul},
  journal={The Visual Computer},
  note={Under Review},
  year={2026}
}
```

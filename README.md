# Hybrid Deep Learning Pipeline for Real-Time Video Analytics  
Detection • Tracking • Background Understanding

**Paper title:** Hybrid Deep Learning Pipeline for Real-Time Video Analytics with Detection, Tracking, and Background Understanding  
**Authors:** Kuldeep Vayadande *(corresponding author)*, and co-authors  
**Affiliation:** Vishwakarma Institute of Technology, Pune  
**Contact (corresponding author):** kuldeep.vayadande@gmail.com  

This repository contains the **exact Colab notebook** used to run our end-to-end pipeline. The notebook installs dependencies, downloads required pretrained weights automatically (where applicable), runs inference, and finally launches a small **Gradio demo link** in the last cell.

---

## What this repo contains
- `vid_analytics.ipynb` – single notebook to run everything on Google Colab

That’s it by design: the goal is to keep replication simple.

---

## Quick start (recommended: Google Colab)
1. Open the notebook in Colab  
   - Upload the notebook to Colab **or** use the “Open in Colab” badge below.

2. In Colab:
   - **Runtime → Change runtime type → GPU** (recommended)
   - Run all cells **top to bottom**

3. In the last cell, a **Gradio public URL** is printed.
   - Click it to open the demo in a new tab.

### Open in Colab badge (edit the notebook name)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/coolss21/Hybrid-Deep-Learning-Video-Analytics/blob/main/NOTEBOOK_NAME.ipynb
)

---

## Environment and dependencies
The notebook is intended for **Google Colab** (tested with GPU runtime).  
Main Python packages used (installed inside the notebook when needed):

- `ultralytics` (YOLO-based detection)
- `deep-sort-realtime` (tracking)
- `transformers` (semantic segmentation models)
- `gradio` (demo UI)
- plus standard Colab packages like `torch`, `opencv-python`, `numpy`, etc.

If you run locally (not recommended for this repo), you’ll need a working CUDA/PyTorch setup and may need to manually align package versions.

---

## Data availability
All datasets used in this study are publicly available from their official sources.  
To support replication, this repository/notebook includes dataset preparation steps and uses the official evaluation splits where provided.  
Datasets that require registration are **not redistributed**.

**Official sources:**
- MS-COCO 2017: https://cocodataset.org/
- MOT17: https://motchallenge.net/data/MOT17/
- ADE20K: https://groups.csail.mit.edu/vision/datasets/ADE20K/
- BDD100K: https://bdd-data.berkeley.edu/
- Cityscapes (registration required): https://www.cityscapes-dataset.com/

> Note: Some datasets have license and registration requirements. Please follow each dataset’s official terms.

---

## Code availability 
The full implementation used for the experiments is available in this public repository as a runnable Google Colab notebook:
- https://github.com/coolss21/Hybrid-Deep-Learning-Video-Analytics

---

## Reproducibility notes
- For best results, run on **Colab T4 GPU** and execute cells in order.
- If the notebook downloads any external weights/models, Colab may cache them across runs.
- If your results differ slightly (FPS / timing), that can happen due to GPU type differences on Colab.

---

## How to cite
If you use this code, please cite our paper.

**BibTeX (update once accepted / published):**
```bibtex
@article{vayadande2026hybrid,
  title   = {Hybrid Deep Learning Pipeline for Real-Time Video Analytics with Detection, Tracking, and Background Understanding},
  author  = {Vayadande, Kuldeep and others},
  journal = {Pattern Analysis and Applications},
  year    = {2026},
  note    = {Under review / Accepted / Published (update this)},
}

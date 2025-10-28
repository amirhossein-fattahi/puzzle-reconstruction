# 🧩 Puzzle Reconstruction Using Computer Vision

[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)]()
[![OpenCV](https://img.shields.io/badge/opencv-4.x-green.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 📖 Project Overview
This project implements a **computer vision pipeline** to automatically reconstruct a jigsaw puzzle from input images.  
It was developed as part of the **Computer Vision course (2024/25), University of Padova**.

The pipeline combines:
- **Segmentation** of puzzle pieces (adaptive thresholding, contours, masks)  
- **Feature extraction & matching** using SIFT + FLANN with Lowe’s ratio test  
- **Homography estimation** with RANSAC for robust geometric alignment  
- **Warping & overlaying** of pieces to assemble the final puzzle  

The system is robust against distortions, irregular shapes, and noise, achieving near-perfect puzzle reconstruction.

📄 See the full [Report.pdf](./report/Report.pdf) for details, methods, and results.

---

## 🚀 Usage
Clone the repository and install dependencies:
```bash
git clone https://github.com/amirhossein-fattahi/puzzle-reconstruction.git
cd puzzle-reconstruction
```

---

## 📊 Results

- **Segmentation accuracy:** All pieces extracted correctly
- **Feature matching success:** ~95% valid homographies
- **Final reconstruction:** Accurate placement, minimal artifacts
- **Warping & overlaying** of pieces to assemble the final puzzle  

Example output (see ./results for more):

- **Segmented puzzle pieces**
- **Feature matching visualizations**
- **Final assembled puzzle image**  



| Segment 1 | Segment 2 | Segment 3 |
|------------|------------|------------|
| ![seg1](./results/segment_detection1.png) | ![seg2](./results/segment_detection2.png) | ![seg3](./results/segment_detection3.png) |

| Result 1 | Result 2 | Result 3 |
|------------|------------|------------|
| ![res1](./results/final_result1.png) | ![res2](./results/final_result2.png) | ![res3](./results/final_result3.png) |

Feature Matching
![feature](./results/feature_matching_31.png)  

---  

## 🧠 Key Metrics

Segmentation accuracy: All pieces extracted correctly  

Feature matching success: ~95% valid homographies  

Final reconstruction: Accurate placement, minimal artifacts  

---  

## 📚 Reference

If you use or modify this project, please cite it or link back to this repository.  

Author: Amirhossein Fattahi
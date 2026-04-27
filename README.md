# 3D Gaussian Splatting — Real-Time Novel View Synthesis
### STA306 Statistical Computing Project (2026)

## Overview
This project implements **3D Gaussian Splatting** (Kerbl et al., SIGGRAPH 2023) 
for real-time novel view synthesis on the Playroom scene from the 
Tanks & Temples / Deep Blending dataset.

## Results

### Training Metrics
| Iteration | PSNR | Loss |
|-----------|------|------|
| 7,000 | 32.15 | 0.0227 |
| 15,000 | — | 0.0135 |
| 30,000 | **36.46** | **0.0097** |

### Rendered Scene
[Add your rendered image here]

## Dataset
- **Scene:** Playroom (Deep Blending dataset)
- **Images:** 225 training images
- **Source:** [3DGS Project Page](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)

## Method
3D Gaussian Splatting represents scenes as millions of tiny 3D Gaussian 
ellipsoids, each with position, shape, color and opacity. These are 
optimized from multi-view photos and rendered in real-time by "splatting" 
them onto a 2D screen.

## How to Run
1. Open `Dwarkesh_3DGS.ipynb` in Google Colab
2. Set runtime to T4 GPU
3. Run all cells in order

## Training Configuration
- Iterations: 30,000
- Resolution: 4x downscale
- Checkpoints: 7000, 15000, 30000

## Reference
Kerbl et al., *3D Gaussian Splatting for Real-Time Radiance Field Rendering*, 
SIGGRAPH 2023. [Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)

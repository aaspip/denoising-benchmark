# denoising-benchmark

<p align="center">
<b>A curated collection of benchmark datasets, reproducible examples, and baseline workflows for seismic denoising research.</b>
</p>

<p align="center">
Designed for benchmarking classical signal processing, sparse transforms, inverse problems, and modern AI/deep learning denoising methods on both synthetic and field seismic datasets.
</p>

---

## Overview

`denoising-benchmark` provides a unified benchmark platform for evaluating seismic denoising algorithms under diverse geological settings, acquisition conditions, and noise characteristics. The repository includes carefully designed synthetic datasets together with representative real seismic examples that challenge existing denoising approaches.

The project aims to support:

- Reproducible research in seismic denoising
- Fair comparison between conventional and AI-based methods
- Benchmarking under coherent and incoherent noise scenarios
- Development of scalable 2D/3D denoising workflows
- Education and methodological validation for geophysical inverse problems

The benchmark is suitable for evaluating:

- Dictionary learning methods
- Sparse transform methods
- Low-rank and rank-reduction methods
- Deep learning denoisers
- Diffusion models
- Self-supervised denoising
- Physics-informed denoising
- Bayesian denoising methods
- Hybrid signal processing + AI workflows

---

# Repository Structure

```text
denoising-benchmark/
│
├── amir3d/        # 3D synthetic incoherent-noise benchmark
├── hyper4/        # 3D synthetic incoherent-noise benchmark
├── coh2d/         # 2D synthetic coherent-noise benchmark
├── edge/          # 2D synthetic edge-preserving benchmark
├── sigmoid/       # Synthetic nonlinear structural benchmark
├── viking2d/      # Real 2D multiple attenuation benchmark
├── sean3d/        # Real 3D interpolation/denoising benchmark
│
└── README.md
```

---

# Scientific Motivation

Seismic denoising remains a fundamental challenge in exploration geophysics, earthquake seismology, and subsurface imaging. Modern acquisition systems generate increasingly large and complex datasets contaminated by:

- Random noise
- Coherent noise
- Multiples
- Acquisition footprint
- Missing traces
- Irregular sampling
- Field acquisition artifacts

While numerous denoising algorithms have been proposed, quantitative comparison across methods is often difficult due to the lack of standardized benchmark datasets and reproducible workflows.

This repository addresses that gap by providing:

✅ Standardized datasets  
✅ Reproducible notebooks  
✅ Representative synthetic and field data  
✅ 2D and 3D benchmarks  
✅ Diverse noise types  
✅ Common evaluation scenarios  

The benchmark can serve as a common testing platform for future developments in:

- AI-assisted seismic processing
- Physics-guided deep learning
- Foundation models for geophysics
- Self-supervised denoising
- Uncertainty-aware denoising
- Real-time seismic monitoring

---

# Benchmark Datasets

| Dataset | Dimension | Type | Main Task | Description |
|---|---|---|---|---|
| `amir3d` | 3D | Synthetic | Random-noise suppression | Complex structural synthetic benchmark with incoherent noise |
| `hyper4` | 3D | Synthetic | Random-noise suppression | Hyperbolic-event benchmark for 3D denoising validation |
| `coh2d` | 2D | Synthetic | Coherent-noise attenuation | Benchmark for coherent noise and linear events |
| `edge` | 2D | Synthetic | Edge-preserving denoising | Tests structural preservation capability |
| `sigmoid` | 2D | Synthetic | Nonlinear structural denoising | Sigmoid-shaped events with incoherent noise |
| `viking2d` | 2D | Real | Multiple attenuation | Real marine seismic benchmark |
| `sean3d` | 3D | Real | Interpolation + denoising | Real 3D seismic interpolation benchmark |

---

# Dataset Gallery

## 1. `amir3d`

3D synthetic benchmark with complex seismic structures contaminated by incoherent noise.

Notebook:  
[amir3d notebook](https://github.com/aaspip/denoising-benchmark/blob/main/amir3d/amir3d.ipynb)

<p align="center">
<img src="https://github.com/aaspip/gallery/blob/main/denoising-benchmark/amir3d.png" width="960"/>
</p>

---

## 2. `hyper4`

3D synthetic hyperbolic-event denoising benchmark.

Notebook:  
[hyper4 notebook](https://github.com/aaspip/denoising-benchmark/blob/main/hyper4/hyper4.ipynb)

<p align="center">
<img src="https://github.com/aaspip/gallery/blob/main/denoising-benchmark/hyper4.png" width="960"/>
</p>

---

## 3. `coh2d`

2D coherent-noise attenuation benchmark for evaluating structure-preserving denoising methods.

Notebook:  
[coh2d notebook](https://github.com/aaspip/denoising-benchmark/blob/main/coh2d/coh2d.ipynb)

---

## 4. `edge`

2D edge-preserving denoising benchmark emphasizing discontinuity preservation.

Notebook:  
[edge notebook](https://github.com/aaspip/denoising-benchmark/blob/main/edge/edge.ipynb)

---

## 5. `sigmoid`

Synthetic nonlinear seismic benchmark with sigmoid-shaped events and incoherent noise contamination.

Notebook:  
[sigmoid notebook](https://github.com/aaspip/denoising-benchmark/blob/main/sigmoid/sigmoid.ipynb)

---

## 6. `viking2d`

Real marine seismic benchmark for multiple attenuation and field-data denoising evaluation.

Notebook:  
[viking2d notebook](https://github.com/aaspip/denoising-benchmark/blob/main/viking2d/viking2d.ipynb)

---

## 7. `sean3d`

Real 3D seismic benchmark for interpolation and denoising research.

Notebook:  
[sean3d notebook](https://github.com/aaspip/denoising-benchmark/blob/main/sean3d/sean3d.ipynb)

---

# Example Applications

The benchmark datasets can be used for:

- Seismic random-noise attenuation
- Coherent-noise suppression
- Multiple attenuation
- Trace interpolation
- Self-supervised denoising
- Diffusion-model training
- Bayesian denoising
- Sparse transform benchmarking
- AI foundation-model evaluation
- Physics-informed neural networks
- Uncertainty quantification studies

---

# Reproducibility

Each benchmark includes:

- Data generation scripts or notebooks
- Visualization examples
- Reproducible workflows
- Ready-to-run benchmark cases

The repository emphasizes transparent and reproducible research practices for the geophysical signal processing community.

---

# Recommended Citation

If you use this repository in your research, please consider citing:

```bibtex
@misc{denoisingbenchmark,
  title={denoising-benchmark: A Collection of Benchmark Datasets for Seismic Denoising},
  author={Yangkang Chen and collaborators},
  year={2026},
  publisher={GitHub},
  howpublished={\url{https://github.com/aaspip/denoising-benchmark}}
}
```

---

# Related Projects

- [AASPIP GitHub Organization](https://github.com/aaspip)
- [Gallery Repository](https://github.com/aaspip/gallery)

---

# Contributing

Contributions are welcome!

Potential contributions include:

- New benchmark datasets
- Additional denoising baselines
- Deep learning workflows
- Evaluation metrics
- Reproducible notebooks
- Benchmark leaderboards

Please feel free to open issues or submit pull requests.

---

# License

This project is released under the MIT License.

---

<p align="center">
<b>Advancing reproducible seismic denoising research through open benchmarks.</b>
</p>

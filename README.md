# Mathematical Models and Methods for Image Processing (MMMIP)

**Politecnico di Milano** — A.Y. 2025/2026  
**Prof.** Giacomo Boracchi
**Credits:** 5 CFU | **Campus:** Milano Leonardo

> Course page: [boracchi.faculty.polimi.it/teaching/MMMIP.htm](https://boracchi.faculty.polimi.it/teaching/MMMIP.htm)

---

## Course Overview

The primary goal of this laboratory course is to let students **design, implement and practice algorithms** based on simple mathematical models from linear algebra and convex optimization, and solve challenging **inverse problems in image processing** (denoising, deblurring, inpainting, anomaly detection).

No neural networks — only expert-driven algorithms with clear mathematical modeling that admit closed-form solutions and sound optimization schemes.

## Topics

| # | Topic | Notebook |
|---|-------|----------|
| 1 | Representation w.r.t. Orthonormal Basis | `lez_1_orthonormal_basis.ipynb` |
| 2 | DCT Basis for Images & Image Compression (JPEG) | `lez_2_DCT_images.ipynb` |
| 3 | Image Denoising: Sliding DCT | `lez_3_DCT_denoising.ipynb` |
| 4 | Wiener Filter & Limitations of Sparsity | `lez_4_limitations_of_sparsity.ipynb` |
| 5 | Away From Orthonormal Basis — PCA Denoising | `lez_5_Global_PCA_denoising.ipynb` |
| 6 | Sparse Coding (OMP, ISTA, IRLS, LASSO) | *TBD* |
| 7 | Dictionary Learning (K-SVD) | *TBD* |
| 8 | Applications: Inpainting, Anomaly Detection, Classification | *TBD* |
| 9 | Robust Fitting (RANSAC, LMEDS, Hough Transform) | *TBD* |

### Full syllabus

- Image models based on orthonormal bases (Fourier, Wavelets), data-driven bases (PCA, Gram-Schmidt) and local polynomial approximation
- Sparsity and redundancy
- Redundant sets of generators (away from orthonormal basis)
- Sparse coding with ℓ₀ (OMP) or ℓ₁ norm (convex optimization — ISTA, IRLS, LASSO)
- Dictionaries yielding sparse representations and dictionary learning (K-SVD)
- Applications of sparse models to image denoising, inpainting, anomaly detection and classification
- Robust fitting methods (RANSAC, LMEDS, Hough) and sequential counterparts for object detection

## Repository Structure

```
MMMIP/
├── notebooks/          # Jupyter notebooks — lab assignments & solutions
├── data/               # Test images and .mat data files
├── slides/             # Lecture slides (PDF)
├── .gitignore
└── README.md
```

## Prerequisites

- **Math:** Linear Algebra, Statistics, Calculus
- **Programming:** Python (or MATLAB)
- **Libraries:** NumPy, SciPy, Matplotlib, scikit-image

## Resources

- [Course Introduction Slides (PDF)](https://boracchi.faculty.polimi.it/teaching/MMMIP/MMMIP_Boracchi_Introduction.pdf)
- [Colab Assignments Folder](https://drive.google.com/drive/folders/16h7wXQZOk1MQScu7iPJwYinlvPnvNMPP?usp=sharing)
- [Course Calendar](https://boracchi.faculty.polimi.it/teaching/MMMIPCalendar.htm)

## License

Educational use only. Course materials belong to Prof. Giacomo Boracchi / Politecnico di Milano.

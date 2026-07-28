# Mathematical Models and Methods for Image Processing (MMMIP)

**Politecnico di Milano** — A.Y. 2025/2026  
**Prof.** Giacomo Boracchi

> Course page: [boracchi.faculty.polimi.it/teaching/MMMIP.htm](https://boracchi.faculty.polimi.it/teaching/MMMIP.htm)

---

## Course Overview

The primary goal of this laboratory course is to let students **design, implement and practice algorithms** based on simple mathematical models from linear algebra and convex optimization, and solve challenging **inverse problems in image processing** (denoising, deblurring, inpainting, anomaly detection).

No neural networks — only expert-driven algorithms with clear mathematical modeling that admit closed-form solutions and sound optimization schemes.

## Topics

| # | Topic | Notebook | Description |
|---|-------|----------|-------------|
| 1 | Representation w.r.t. Orthonormal Basis | `lez_01_orthonormal_basis.ipynb` | Builds and analyzes 1D DCT bases, orthogonality, projections and sparse coefficients. |
| 2 | DCT Basis for Images & Image Compression (JPEG) | `lez_02_DCT_images.ipynb` | Introduces 2D DCT dictionaries for image patches and JPEG-style compression/reconstruction. |
| 3 | Image Denoising: Sliding DCT | `lez_03_DCT_denoising.ipynb` | Implements image denoising with smoothing, patchwise DCT sparsity, hard thresholding and Wiener filtering. |
| 4 | Away From Orthonormal Bases & Limitations of Sparsity | `lez_04_limitations_of_sparsity.ipynb` | Compares sparsity in orthonormal and redundant dictionaries, with denoising and Tikhonov regularization examples. |
| 5 | PCA Denoising | `lez_05_Global_PCA_denoising.ipynb` | Uses PCA/data-driven bases to denoise images from noisy patch observations. |
| 6 | Matching Pursuit | `lez_06_matching_pursuit.ipynb` | Implements greedy sparse approximation with Matching Pursuit over redundant dictionaries. |
| 7 | Matching Pursuit Variants | `lez_07_matching_pursuit_variants.ipynb` | Extends the sparse coding workflow with alternative pursuit strategies and coefficient updates. |
| 8 | Sparse Inpainting | `lez_08_Inpainting.ipynb` | Restores missing image pixels by combining patch dictionaries, masks and OMP-based sparse reconstruction. |
| 9 | OMP Denoising | `lez_09_OMP_Denoising.ipynb` | Applies Orthogonal Matching Pursuit to patch-based image denoising with redundant dictionaries. |
| 10 | Dictionary Learning (K-SVD) | `lez_10_KSVD.ipynb` | Learns dictionaries from image patches with K-SVD and uses them for OMP denoising and texture modeling. |
| 11 | Gradient Descent | `lez_11_gradient_descent.ipynb` | Studies least-squares optimization, objective visualization and iterative gradient descent updates. |
| 12 | Non-Local Means & Self-Similarity | `lez_12_NLMeans.ipynb` | Explores image self-similarity and implements Non-Local Means denoising. |
| 13 | ISTA | `lez_13_ISTA.ipynb` | Solves L1-regularized sparse coding/LASSO problems with the Iterative Shrinkage-Thresholding Algorithm. |
| 14 | FISTA | `lez_14_FISTA.ipynb` | Accelerates ISTA with FISTA momentum for faster L1-regularized optimization. |
| 15 | IRLS, MOD & L1 Denoising | `lez_15_IRLS_MOD_l1Denoising.ipynb` | Compares IRLS and FISTA for L1 sparse coding and applies the workflow to dictionary-based denoising. |
| 16 | Sparse Anomaly Detection | `lez_16_Anomaly_Detection.ipynb` | Detects anomalies by learning a normal dictionary, estimating sparse reconstruction errors and thresholding detections. |
| 17 | Local Polynomial Approximation (LPA) | `lez_17_LPA.ipynb` | Builds standard and weighted LPA kernels and applies centered, left and right filters to synthetic signals. |
| 18 | Adaptive LPA-ICI | `lez_18_LPA_ICI.ipynb` | Selects the local scale adaptively with the ICI rule and combines left- and right-sided estimates through aggregation. |
| 19 | 2D and Anisotropic LPA-ICI | `lez_19_LPA_ICI_2D.ipynb` | Extends LPA-ICI to image denoising with multiscale isotropic and directional kernels, selected scales and PSNR evaluation. |
| 20 | Robust Fitting | `lez_20_Robust_Fitting.ipynb` | Compares OLS and DLT line fitting under outliers and implements RANSAC, MSAC and LMedS robust estimators. |
| 21 | Multi-Model Fitting | `lez_21_Multi_Model_Fitting.ipynb` | Uses Sequential RANSAC to detect multiple lines and circles in the Stair, Star and circle datasets. |

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

## License

Educational use only. Course materials belong to Prof. Giacomo Boracchi / Politecnico di Milano.

## Valutazione

**10/10**

# notebooks

ML and DL related Google Colab notebooks.

## Outline

### Learning algorithms

- `grad_descent.ipynb` — Steps down \(f(x_1, x_2) = x_1^2 + b x_2^2\) with a fixed learning rate and plots the path on an elliptic contour.
- `linear_regression.ipynb` — Draws a noisy one-feature regression sample of 100 points and plots it.
- `k_means.ipynb` — Runs k-means from scratch on 1,000 points in three 2D blobs and plots the clusters with their centroids.

### Signals and images

- `image_processing.ipynb` — Loads the 512×512 Lena image and applies a hard threshold at 128, turning it into a black-and-white bitmap. The writeup sets that cutoff against Haar, DB4, and Meyer wavelet compression.
- `TransientDetector.ipynb` — Builds noisy 128-sample waveforms, sometimes with a short transient, and trains a 1D CNN and a depthwise-separable CNN to detect it.
- `Transient_CNN_MLP.ipynb` — Uses the same transient signals. An MLP classifies Haar-wavelet features, and a 1D CNN classifies the raw waveform.

### Networks, lookup tables, and fixed point

- `nn_vs_lut_multi_d.ipynb` — Approximates 1D, 2D, and 3D target functions with lookup tables of size 32 and 64, and with a hybrid that adds a small residual network.
- `NN_Hybrid_Using_LUT_Xipynb.ipynb` — Interpolates a lookup table and trains a 2×8 residual network on the error, including a case that feeds the table value in as an extra input.
- `Fixed_Point_NN.ipynb` — Trains a small network on 1D, 2D, and 3D functions using floating-point inputs, fixed-point inputs, and both together, then plots the fixed-point error against the hybrid.

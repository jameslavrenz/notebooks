# notebooks

DSP, Controls & AI related Google Colab notebooks.

## Engineering Highlights

- **Embedded-oriented numerical trade-offs:** Notebook experiments compare lookup tables, compact residual neural networks, and mixed approaches for one- to three-dimensional functions ([LUT / NN comparison](nn_vs_lut_multi_d.ipynb), [hybrid LUT model](NN_Hybrid_Using_LUT_Xipynb.ipynb)).
- **Fixed-point exploration:** Evaluates floating-point versus fixed-point inputs and examines approximation errors in small neural networks ([fixed-point notebook](Fixed_Point_NN.ipynb)).
- **Signal detection experiments:** Compares CNN and depthwise-separable CNN approaches on synthetic noisy transients, and MLP classification using Haar-wavelet features ([transient detector](TransientDetector.ipynb), [CNN/MLP comparison](Transient_CNN_MLP.ipynb)).
- **Foundational algorithms:** Includes from-scratch examples for gradient descent, linear regression, and k-means clustering ([algorithm notebooks](#learning-algorithms)).
- **Evidence boundary:** These are **exploratory Colab notebooks**, not measured MCU firmware, hardware benchmarks, or a packaged CI-tested library; see each notebook for its assumptions, code, and plots.

## Outline

### Networks, lookup tables, and fixed point

- `nn_vs_lut_multi_d.ipynb` — Approximates 1D, 2D, and 3D target functions with lookup tables of size 32 and 64, and with a hybrid that adds a small residual network.
- `NN_Hybrid_Using_LUT_Xipynb.ipynb` — Interpolates a lookup table and trains a 2×8 residual network on the error, including a case that feeds the table value in as an extra input.
- `Fixed_Point_NN.ipynb` — Trains a small network on 1D, 2D, and 3D functions using floating-point inputs, fixed-point inputs, and both together, then plots the fixed-point error against the hybrid.

### Signals and images

- `image_processing.ipynb` — Loads the 512×512 Lena image and applies a hard threshold at 128, turning it into a black-and-white bitmap. The writeup sets that cutoff against Haar, DB4, and Meyer wavelet compression.
- `TransientDetector.ipynb` — Builds noisy 128-sample waveforms, sometimes with a short transient, and trains a 1D CNN and a depthwise-separable CNN to detect it.
- `Transient_CNN_MLP.ipynb` — Uses the same transient signals. An MLP classifies Haar-wavelet features, and a 1D CNN classifies the raw waveform.

### Learning algorithms

- `grad_descent.ipynb` — Steps down \(f(x_1, x_2) = x_1^2 + b x_2^2\) with a fixed learning rate and plots the path on an elliptic contour.
- `linear_regression.ipynb` — Draws a noisy one-feature regression sample of 100 points and plots it.
- `k_means.ipynb` — Runs k-means from scratch on 1,000 points in three 2D blobs and plots the clusters with their centroids.

# Parallel PDE Solvers

Numerical implementations demonstrating high-performance techniques for solving partial differential equations. The focus is on finite difference methods with CPU and GPU acceleration using Python, Numba, and CUDA.

## Overview

This repository contains four self-contained Jupyter notebooks that implement and benchmark different numerical approaches to common PDE problems. Each notebook includes mathematical derivations, implementation details, and performance analysis across different hardware architectures.
The notebooks are designed to be educational, showing both the mathematical foundations and practical implementation considerations for high-performance PDE solving.

## Notebooks

| Notebook | Problem Type | Key Methods | Focus |
|----------|-------------|-------------|--------|
| **Diffusion-PDE.ipynb** | 2D Heat Equation | Forward/Backward Euler | Stability analysis, CUDA optimization |
| **Poisson-PDE.ipynb** | Elliptic PDE | 5-point stencil | Sparse matrices, GPU memory optimization |
| **Helmholtz-PDE.ipynb** | Modified Helmholtz | Conjugate Gradient | Iterative solvers, convergence analysis |
| **Diffusion-Iteration.ipynb** | Diffusion Process | Numba acceleration | Performance benchmarking, parallelization |


## Implementation Details

The implementations demonstrate several key computational techniques:

- **Finite difference discretization** on regular grids with proper boundary condition handling
- **Stability analysis** for explicit time-stepping schemes  
- **Sparse matrix construction** and solution for implicit methods
- **GPU memory optimization** using shared memory to reduce global memory access
- **JIT compilation** with Numba for near-C performance from Python
- **Parallel processing** using multi-core CPU capabilities

Performance results show that GPU acceleration becomes advantageous for sufficiently large problem sizes, with the CUDA implementations achieving substantial speedups over CPU methods for equivalent accuracy. The notebooks include detailed timing comparisons and scaling analysis.

## Dependencies

- Python 3.7+
- NumPy, SciPy, Matplotlib  
- Numba (for JIT compilation and CUDA kernels)
- Jupyter

GPU examples require NVIDIA hardware with CUDA support.

# Parallel PDE Solvers

> **Note:** A condensed set of notes and applied problems from the [Techniques of High-Performance Computing](https://tbetcke.github.io/hpc_lecture_notes/intro.html) module at UCL.


Numerical implementations demonstrating high-performance techniques for solving partial differential equations. The focus is on finite difference methods with CPU and GPU acceleration using Python, Numba, and CUDA.

## Overview

This repository contains four self-contained Jupyter notebooks that implement and benchmark different numerical approaches to common PDE problems. Each notebook includes mathematical derivations, implementation details, and performance analysis across different hardware architectures.

## Notebooks

| Notebook | Problem Type | Key Methods | Focus |
|----------|-------------|-------------|--------|
| **Diffusion-PDE.ipynb** | 2D Heat Equation | Forward/Backward Euler | Stability analysis, CUDA optimization |
| **Poisson-PDE.ipynb** | Elliptic PDE | 5-point stencil | Sparse matrices, GPU memory optimization |
| **Helmholtz-PDE.ipynb** | Modified Helmholtz | Conjugate Gradient | Iterative solvers, convergence analysis |
| **Diffusion-Iteration.ipynb** | Diffusion Process | Numba acceleration | Performance benchmarking, parallelization |


## Dependencies

- Python 3.7+
- NumPy, SciPy, Matplotlib  
- Numba (for JIT compilation and CUDA kernels)
- Jupyter

GPU examples require NVIDIA hardware with CUDA support.

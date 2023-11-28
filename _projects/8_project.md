---
layout: page
title: AMX/GPU + Pre
description: Approximate solutions and preconditioning using AMX, AVX and Tensor Cores
img: assets/img/stokes.jpg
importance: 1
category: undergrad
---

# Description

**This project is intended as a full year Honours project and a scholarship is
available to the right candidate.**

Many large scale numerical problems involve the solution of large
systems of equations using iterative techniques that require a number
of repeated solutions to eventually converge to a required
tolerance. Recent hardware developments, primarily intended to
accelerate machine learning training, have introduced the capability
to perform small matrix operations rapidly but at reduced precision.

Recently, several attempts have been made to co-opt these
architectural advances for numerical computing problems with some
success (see references below).

The two main hardware developments (available on Gadi) are

- AMX BF16 and AVX512 FP16 extensions available on the Sapphire Rapids microarchitecture
- CUDA Tensor Cores available on multiple generations of NVidia Compute/Graphics cards

This project would look at applying one or more of these hardware accelerated
low precision matrix multiplications to numerical
problems implemented with the spectral element method (SEM). The SEM
uses an efficient tensorized expansion that is well suited to
implementation using local small matrix operations. Two aspects will be explored:

- firstly, can we achieve reasonable results from a direct solution of a SEM problem
using one or more of these low precision accelerators (potentially with additional problem
rescaling), and secondly,
- how can we use these for rapid pre-conditioning of iterative solvers in an HPC environment.


# Pre-requisites

- C/C++, Python
- HPC (COMP3320, COMP4300)
- Some basic mathematical knowledge would be required

# References

- [Anzt, H. et al, "Adaptive precision in block-Jacobi preconditioning for iterative sparse linear system solvers", Concurrency Computat Pract Exper., 2019](https://doi.org/10.1002/cpe.4460)
- [Ina, T. et al, "A new data conversion method for mixed precision Krylov solvers with FP16/BF16 Jacobi preconditioners", HPC Asia, 2023](https://doi.org/10.1145/3578178.3578222)
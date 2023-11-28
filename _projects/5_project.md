---
layout: page
title: soft+sem
description: Soft spectral element method (softSEM) and its application to seismic wave simulation 
img: assets/img/mesh.jpg
importance: 3
category: pastproject
---

Completed by Heming Zhu 2023

The high-order spectral element method (SEM) has been widely used in geoscience for simulating seismic waves.
However, like the higher-order finite element methods (FEMs), high-order SEMs suffer from high stiffness
(large condition numbers) in their discretized systems. Following the softFEM idea, we propose to reduce the
stiffness of the problem by subtracting a least-squares penalty on the gradient jumps across the mesh interfaces
from the standard stiffness SEM bilinear form. We refer to this method as softSEM. The two key goals of softSEM
are (1) to reduce the numerical dispersion errors, especially for high-frequency waves, leading to more accurate
simulation; and (2) to reduce the condition number (i.e., the stiffness) of the discretized system, leading to
larger time-marching step size when using explicit schemes and hence computational advantages. The major
difficulty of this project is to optimize the softness parameter such that the resulting system is coercive while the above goals are achieved.

We will provide a basic code (both Python and Matlab codes are available for your choice) for this project.

# Pre-requisites

Although not mandatory, some mathematical knowledge or numerical modelling knowledge would be desirable.

Use of HPC resources (e.g., Gadi) may be advantageous

# Notes

This project is ideal for an Honour’s or Master’s student pursuing 12 or 24 units over two consecutive semesters.

# Supervisors

- [Dr Quanling Deng (SOCO)](https://comp.anu.edu.au/people/quanling-deng/)
- [Dr Rhys Hawkins (SOCO)](https://comp.anu.edu.au/people/rhys-hawkins/)

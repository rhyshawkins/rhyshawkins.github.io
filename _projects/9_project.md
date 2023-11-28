---
layout: page
title: AMR-SPEC
description: Adaptive Mesh Refinement for Spectral Element problems
img: assets/img/mesh-zoom.png
importance: 1
category: undergrad
---

# Description

**This project is intended as a full year Honours project and a scholarship is
available to the right candidate.**

The spectral element method (SEM) is a widely used variant of finite
elements adapted to quadrilateral (2D) or hexahedral (3D)
elements. It's advantages are that it is relatively simple to
implement, the use of tensorized bases in higher dimensions is
computationally efficient including higher order elements, and it
produces a diagonal mass matrix which is useful for explicit solutions
of time varying problems.

The down side of the use of quads or hex elements is that meshes are
difficult to construct automatically. In addition, when there is a
sharp change in material properties, e.g. ground - atmosphere,
traditional spectral element meshes are highly inefficient.

There have been recent attempts at incoporating Adaptive Mesh
Refinement (AMR) into standard spectral element codes. The core of
technique required by these methods are non-conforming spectral
elements, where the edges/faces of neighboring elements do not
precisely align. Non-conforming meshes allow greater flexibility and simplicity in mesh
generation, but a large problem is that the mass matrix will no longer
be diagonal, rather it will be block diagonal and therefore more
difficult to invert.

This project will examine accuracy and performance issues of an
implementation of spectral elements with non-conforming cells in time
varying problems at different scales.

The target application is in geophysical modelling where we often have
sharp changes in material properties, for example, ground-atmosphere
or mantle-outer core.

# Pre-requisites

- C/C++, Python 
- HPC (COMP3320, COMP4300) experience

# References

- [N. Offermans et al, "Towards adaptive mesh refinement for the spectral element solver Nek5000", Proceedings DLES11, 2017](https://link.springer.com/chapter/10.1007/978-3-030-04915-7_2)

# Supervisors

- [Dr Rhys Hawkins (SOCO)](https://comp.anu.edu.au/people/rhys-hawkins/)
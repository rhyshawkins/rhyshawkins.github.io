---
layout: page
title: hpc+eigen
description: Approaches to large scale solution of non-linear eigen problems.
img: assets/img/eigen.jpg
importance: 3
category: undergrad
---

In many fields of science and engineering, the eigen solutions of physical
equations have important applications in many fields.

Examples from structural analysis include the Tacoma Narrows bridge
where a relatively mild wind excited torsional vibration modes of a
bridge that subsequently resulted in its eventual [collapse](https://en.wikipedia.org/wiki/Tacoma_Narrows_Bridge_(1940)).

An example from seismology include using passive techniques that
``listen'' for fundamental eigen modes at different frequencies. From
this information, the subsurface structure and its likelihood to shake
severely during an Earthquake can be inferred.

The traditional calculation of eigen solutions is well established but
scales very poorly and cannot be used for large scale problems.
Fortunately, in many cases, we only require a small number of eigen
solutions rather than the whole spectrum and there have been many
algorithms developed over the years that efficiently compute a small
subset of eigen solutions.  A recent advance is the so called FEAST
algorithm with its additional benefit being that
it can also operate on polynomial and non-linear eigen problems.

This honours project would examine the application of High Performance
Computing strategies for solving larger scale non-linear eigen
problems.

# Prerequisites

This project would require a working knowledge of basic linear algebra.

Although not mandatory, some mathematical knowledge or numerical modelling knowledge would be desirable.

Use of HPC resources (e.g., Gadi) would be advantageous

# Notes

This project is ideal for an Honour’s or Master’s student pursuing 12 or 24 units over two consecutive semesters.

# Supervisors

- [Dr Rhys Hawkins (SOCO)](https://comp.anu.edu.au/people/rhys-hawkins/)


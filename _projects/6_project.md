---
layout: page
title: PhD 
description: PhD involving numerical simulation, approximation, and inference
img: assets/img/earthimage.jpg
importance: 4
category: phd
---

# Overview

I do not have any open positions for a PhD at present but if you are
interested in the general topics outlined below then please get in touch.
Please also note the admission deadlines below for the PhD program at the ANU.

## Numerical Simulation and High Performance Computing

For many years, various computationally expensive techniques have been
used for the simulation of complex physical phenomena within the
Earth. An example from seismic tomography is full waveform simulation
for the simulation of the Earths response due to an Earthquake, which
coupled with adjoint simulations, can subsequently be used to infer
the structure of the Earth. These techniques are well established and
have community open source codes that are generally well optimized for
running on super computing resources.

I am generally interested in research around both different methods
for the solution of wave propagation problems (e.g. FEM, SEM, DG etc)
and their efficient implementation on high performance computing
resources.

## Useful Approximations

In addition to high fidelity numerical simulation and advances therein
outlined in the previous section, there is a great deal of interest in
the use for numerical approximation techniques for approximating these
simulations at dramatically reduced costs. Applications for this
include (near) real-time monitoring of physical phenomena, or
evaluating large number of solutions for scenario evaluations.

There are two broad categories that I am interested in: model order
reduction (or reduced basis) methods and machine learning approaches.

On the first hand, model order reduction generally seaks a reduced
basis (subspace) on to which a high fidelity system can be projected
that produces a much lower dimension simulation while maintaining
numerical stability and a high degree of accuracy. The general idea is that
simulations can then be computed with 2-4 orders of magnitude less
expense which incurring moderate approximation errors, i.e. < 1%.

On the other hand, machine learning techniques such as Physically
Informed Neural Networks have been shown to accurately reproduced the
results of partial differential equations under various scenarios.
Some recent work has also shown the use of Auto Encoders that can act
as efficient numerical integrators through time, i.e. they can predict
the state of a numerical system and the next or the previous time
step.


## Bayesian Inference

Much of my early research was in Bayesian inference and in the so-called
Trans-dimensional sampling algorithms. These are based on McMC or HMC sampling
methods that attempt to approximate a posterior probability distribution
using a population of likely models. As problems get larger, McMC/HMC become
progressively less tractable due to the curse of dimensionality.

Primarily for this reason, I am more interested now in optimization techniques
such as Variational Bayes and Generative Models as methods of approximating the
posterior distribution.

# Applying

There are two rounds each year for applying for entry into the PhD Program
at ANU:
 - April (Both Domestic and International Students)
 - October (Domestic Students), August (International Students)
 
Detailed information can be found here:
 - [https://programsandcourses.anu.edu.au/program/9070XPHD](https://programsandcourses.anu.edu.au/program/9070XPHD)

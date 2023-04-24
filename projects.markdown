---
layout: page
title: Projects
permalink: /projects/
---


Each WATCHEP trainee works with a university mentor and DOE laboratory mentor to complete a research project in computational high-energy physics.
This page gives a list of current and future projects suggested by DOE lab mentors.


## Hardware-Software Co-Design

* **Optimizing FPGA algorithms and host-kernel data transfer.**
    FPGAs can be used for online event filter tracking. One implementation of the Hough Transform is the 1D bitshift Hough Transform, designed to make use of the FPGA architecture and parallel processing. The goal is to provided generic host code to load kernels across FPGAs, GPUs, and maintain instruction queues and data transfer queues to coordinate activities across the different architectures. Trainee: Eric Le (UCI). Mentor: Viviana Cavaliere (BNL).
* **Identifying boosted H&rarr;cc decays with GNNs.**
GNNs are a natural solution to the flavor-tagging problem, since a large radius jet can be represented as a fully connected graph with each track in the jet corresponding to a single node in the graph.
The goal is to aid in the creaIon of an algorithm to idenIfy boosted H->cc decays.
Trainee: Johannes Wagner. Mentor: Simone Pagan Griso (LBNL)
* **High-Speed Data Acquisition Using PCIe FPGA Cards**
This project is the development of a FPGA-based readout system for a silicon pixel telescope. Possible improvements on the maximum transfer speed for the system will focus on scaling to more PCIe lanes and migrating to a new PCIe protocol.
Trainee: Luc Le Pottier (UCB).
Mentor: Timon Heim (LBNL).
* **ML algorithms on FPGAs.**
This project is the extension of the fast ML hardware-software codesign tool known as hls4ml by upgrading to the latest high-level synthesis (HLS) language, Vitis HLS. The benefits of using pruning and sparsity to accelerate inference of ML models will also be investigated.
Trainee: Russell Marroquin Solares (UCSD). Mentor: Nhan Tran (FNAL).
* **Simplified task execution scheduler.**
  The goal of this project is to develop a simplified task execution scheduler for ATLAS using C++ asynchronous execution and benchmark its performance.
Trainee: Abdelrahman Elabd (UW). Mentors: Charles Leggett (LBNL), Xiangyang Ju (LBNL).

## Collaborative Software Infrastructure

* **Pipeline Development for LSST DESC.**
    Firecrown is the primary software package responsible for implementing all of the likelihoods to be used within the Dark Energy Science Collaboration and for orchestrating the combination of said likelihoods, priors, and samplers to generate parameter constraints. The goal is to implement an un-binned cluster number counts approach, which is more robust than the typical binned cluster number counts analysis
Trainee: Matt Kwiecien (UCSC). Mentor: Marc Paterno (FNAL).
* **Machine Learning RooUnfold.**  
    Unfolding is one of the main computational tasks across HEP to measure differential cross sections. The most widely used software package for unfolding is RooUnfold. The purpose of this project is to extend RooUnfold to be compatible with modern Machine Learning (ML) libraries to be able to perform unbinned unfolding, a new paradigm that is enabled by advanced in deep learning for HEP. Mentor: Ben Nachman (LBNL)
* **Machine Learning Unfolding at Scale.**
    Recent advances in deep learning have allowed for unbinned and high-dimensional unfolding for the first time.  These approaches are currently limited to relatively small dates because of computational challenges.  The goal of this project is to integrate ML-based unfolding with the Perlmutter GPU supercomputer to use model and data parallelism to push cross section measurements to the next level. Mentors: Ben Nachman (LBNL), Wahid Bhimji (LBNL)

## High-Performance Software and Algorithms

* coming soon...

[jekyll-organization]: https://github.com/watchep

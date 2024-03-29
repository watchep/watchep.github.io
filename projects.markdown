---
layout: page
title: Projects
permalink: /projects/
---


Each WATCHEP trainee works with a university mentor and DOE laboratory mentor to complete a research project in computational high-energy physics.
This page gives a list of current and future projects suggested by DOE lab mentors.


## Hardware-Software Co-Design

* **Optimizing FPGA algorithms and host-kernel data transfer.**
    FPGAs can be used for online event filter tracking. One implementation of the Hough Transform is the 1D bitshift Hough Transform, designed to make use of the FPGA architecture and parallel processing. The goal is to provided generic host code to load kernels across FPGAs, GPUs, and maintain instruction queues and data transfer queues to coordinate activities across the different architectures.
    Trainee: Eric Le (UCI). Mentor: Viviana Cavaliere (BNL).
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
Mentors: Charles Leggett (LBNL), Xiangyang Ju (LBNL).

## Collaborative Software Infrastructure

* **Pipeline Development for LSST DESC.**
    Firecrown is the primary software package responsible for implementing all of the likelihoods to be used within the Dark Energy Science Collaboration and for orchestrating the combination of said likelihoods, priors, and samplers to generate parameter constraints. The goal is to implement an un-binned cluster number counts approach, which is more robust than the typical binned cluster number counts analysis.
Trainee: Matt Kwiecien (UCSC). Mentor: Marc Paterno (FNAL).
* **Machine Learning RooUnfold.**  
    Unfolding is one of the main computational tasks across HEP to measure differential cross sections. The most widely used software package for unfolding is RooUnfold. The purpose of this project is to extend RooUnfold to be compatible with modern Machine Learning (ML) libraries to be able to perform unbinned unfolding, a new paradigm that is enabled by advanced in deep learning for HEP. Mentor: Ben Nachman (LBNL)
* **Machine Learning Unfolding at Scale.**
    Recent advances in deep learning have allowed for unbinned and high-dimensional unfolding for the first time.  These approaches are currently limited to relatively small dates because of computational challenges.  The goal of this project is to integrate ML-based unfolding with the Perlmutter GPU supercomputer to use model and data parallelism to push cross section measurements to the next level. Mentors: Ben Nachman (LBNL), Wahid Bhimji (LBNL)

## High-Performance Software and Algorithms

* **IPUs for Particle Tracking.**
GraphCore IPUs are designed to massively parallel multiple instructions, multiple data, and fine-grained, high-performance computing. The project aims to port existing tracking algorithms (traditional and/or ML-based) to IPUs and compare the computing performance with CPUs and GPUs. Mentors: Xiangyang Ju (LBNL) and Paolo Calafiura (LBNL)
* **High-performance data acquisition software.**
The ATLAS ITk pixel project online software requires high performance to enable gigahertz operation needed for the High-Luminosity LHC. This project would include establishing clean benchmarks, profiling the software, optimizing it, and making this level of performance maintainable during operations. Mentor: Timon Heim (LBNL)
* **Particle flow reconstruction for current and future detectors**
Particle flow reconstruction is one example of combining low-level measurements across detectors. Performance is important to allow all of the inputs to be combined in a reasonable amount of time. This work from project can be relevant for the ATLAS experiment or future experiments.
Mentor: Ben Nachman (LBNL)
* **High-throughput reconstruction/simulation with batched input**
We typically train inference models with batches of events, but we *evaluate* on single events, one at a time. This project would explore the possibility of batch processing on the evaluation side, providing an alternative to the parallel processing event model. 
Mentor: Ben Nachman (LBNL)
* **Track reconstruction as a service.**
Track reconstruction plays a vital role in all physics programs at the Large Hadron Collider and one that is amenable to GPU porting. The project aims to set up a service for track reconstruction using NVIDIA Triton, an open-source software that organizes code deployment and execution across multiple platforms. We will use Triton to execute GPU algorithms from ACTS (a.k.a ACTS as a service), the ExaTrkX Graph Neural Network-based ML pipeline (a.k.a ExaTrkX as a service), or a hybrid. Delivering GPU cycles with the "as a service" model would enable running ATLAS reconstruction transparently on any GRID site, GPU-enabled or not. Mentors: Xiangyang Ju (LBNL) and Paolo Calafiura (LBNL)
* **Language models for particle detectors.**
Language models have revolutionized natural language understanding and communication. Particle detectors are complex apparatuses whose language is made of raw data organized in subdetectors and readout modules.  The project aims to train a language model that understands a detector's vocabulary and can translate its raw data to higher-level constructs like clusters, tracks, jets, etc.  Mentors: Xiangyang Ju (LBNL) and Paolo Calafiura (LBNL)

[jekyll-organization]: https://github.com/watchep

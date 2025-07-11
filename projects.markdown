---
layout: page
title: Projects
permalink: /projects/
---


Each WATCHEP trainee works with a university mentor and DOE laboratory mentor to complete a research project in computational high-energy physics.
This page gives a list of current and future projects suggested by DOE lab mentors.


## Hardware-Software Co-Design

* **Optimizing FPGA algorithms and host-kernel data transfer.**<br>
    FPGAs can be used for online event filter tracking. One implementation of the Hough Transform is the 1D bitshift Hough Transform, designed to make use of the FPGA architecture and parallel processing. The goal is to provide generic host code to load kernels across FPGAs, GPUs, and maintain instruction queues and data transfer queues to coordinate activities across the different architectures.<br>
    *Trainee: Eric Le (UCI). Mentor: Viviana Cavaliere (BNL).*
* **Identifying boosted H&rarr;cc decays with GNNs.**<br>
GNNs are a natural solution to the flavor-tagging problem, since a large radius jet can be represented as a fully connected graph with each track in the jet corresponding to a single node in the graph.
The goal is to aid in the creaIon of an algorithm to idenIfy boosted H->cc decays.<br>
    *Trainee: Johannes Wagner (UCB). Mentor: Simone Pagan Griso (LBNL).*
* **High-Speed Data Acquisition Using PCIe FPGA Cards**<br>
This project is the development of a FPGA-based readout system for a silicon pixel telescope. Possible improvements on the maximum transfer speed for the system will focus on scaling to more PCIe lanes and migrating to a new PCIe protocol.<br>
*Trainee: Luc Le Pottier (UCB).
Mentor: Timon Heim (LBNL).*
* **ML algorithms on FPGAs.**<br>
This project is the extension of the fast ML hardware-software codesign tool known as hls4ml by upgrading to the latest high-level synthesis (HLS) language, Vitis HLS. The benefits of using pruning and sparsity to accelerate inference of ML models will also be investigated.<br>
*Trainee: Russell Marroquin Solares (UCSD). Mentor: Nhan Tran (FNAL).*
* **Track reconstruction as a service.**<br>
Track reconstruction plays a vital role in all physics programs at the Large Hadron Collider and one that is amenable to GPU porting. The project aims to set up a service for track reconstruction using NVIDIA Triton, an open-source software that organizes code deployment and execution across multiple platforms. We will use Triton to execute GPU algorithms from ACTS (a.k.a ACTS as a service), the ExaTrkX Graph Neural Network-based ML pipeline (a.k.a ExaTrkX as a service), or a hybrid. Delivering GPU cycles with the "as a service" model would enable running ATLAS reconstruction transparently on any GRID site, GPU-enabled or not.<br> 
*Trainee: Miles Cochran-Branson (UW). Mentors: Xiangyang Ju (LBNL) and Paolo Calafiura (LBNL).*
* **Global Particle Flow and pion classification.**<br>
Global Particle Flow (GPF) is a method of reconstructing jets in high energy experiments
like ATLAS which promises an improved jet energy resolution through a comprehensive view of
the event. The reconstruction and classification of pions is a complicated but necessary task in
improving GPF algorithms as well as general detector performance. A deep learning approach to pion classification substantially outperforms existing
classification methods, indicating a strong potential for the use of these tools in GPF.<br>
*Trainee: Alex Golub (UW). Mentor: Ben Nachman (SLAC).*
* **Neural Architecture Codesign for Real-Time Anomaly Detection.**<br>
Anomaly detection in the L1 trigger system uses variational autoencoders to find outlier events.
Neural architecture codesign simultaneously considers both the performance of the neural network architecture and its hardware implementation, to ensure that the models are compatible with the hardware and latency constraints of the trigger system. The pipeline will be released as a reusable software package.<br>
*Trainee: Jason Weitz (UCSD). Mentor: Nhan Tran (FNAL).*
* **Improving performance of parallel processing in a digital readout platform.**<br>
The software infrastructure for digital readout can have potential bottlenecks that impede performance for parallel pipelines. This project focuses on tuning software performance for FPGA readout, using the YARR general purpose platform.<br>
*Trainee: Justine Partridge (UCSC). Mentor: Timon Heim (LBNL).*
* **Simplified task execution scheduler.**<br>
  The goal of this project is to develop a simplified task execution scheduler for ATLAS using C++ asynchronous execution and benchmark its performance.<br>
Mentors: Charles Leggett (LBNL), Xiangyang Ju (LBNL).

## Collaborative Software Infrastructure

* **Pipeline Development for LSST DESC.**<br>
    Firecrown is the primary software package responsible for implementing all of the likelihoods to be used within the Dark Energy Science Collaboration and for orchestrating the combination of said likelihoods, priors, and samplers to generate parameter constraints. The goal is to implement an un-binned cluster number counts approach, which is more robust than the typical binned cluster number counts analysis.<br>
*Trainee: Matt Kwiecien (UCSC). Mentor: Marc Paterno (FNAL).*
* **Late Processing of Selected Data for Low-Momentum Tracking.**<br>
Softer particles are significantly more likely
to multiple-scatter, making the combinatorics involved in track reconstruction infeasible to perform within CPU and disk constraints unless such a momentum cutoff is made.
The key tool that enables this method is ATLAS’s EventIndex catalog, which was developed for
Run 2 to link stored data about recorded events at every stage of processing. The longer-term goal is to have this method approved as a standard
ATLAS processing flow in production.<br>
*Trainee: Luke Grossman (UCB). Mentor: Simone Pagan Griso (LBNL).*
* **Detector Modeling and Event Reconstruction in Future Neutrino Detectors.**<br>
This project will implement an end-to-end analysis chain, from data taking through critical optical calibration and detector modeling, followed by event reconstruction, and data
analysis. The software chain will be tailored for new neutrino detectors based on water, water-based liquid scintillator (WbLS), and pure organic liquid scintillator (LS). It will optimize position reconstruction performance in water and WbLS, comparing simulated data against data from the Eos technology demonstrator.<br>
*Trainee: Martina Hebert (UCB). Mentor: Gabriel Orebi Gann (LBNL).*
* **Modeling Strong-Lensing Galaxy Clusters with GIGA-Lens**<br>
Upcoming projects such as LSST are expected to uncover many thousands of strong
lensing objects. Pixel-level modeling of cluster lenses represents a new frontier, essential to the era of big data sky surveys. This project will adapt the GIGA-Lens software for application to strong-lensing galaxy clusters, with a focus on developing interfaces and testing scalability on large-scale datasets.
<br>
*Trainee: Jackson O'Donnell (UCSC). Mentor: David Schlegel (LBNL).*


## High-Performance Software and Algorithms

* **IPUs for Particle Tracking.**<br>
GraphCore IPUs are designed to massively parallel multiple instructions, multiple data, and fine-grained, high-performance computing. The project aims to port existing tracking algorithms (traditional and/or ML-based) to IPUs and compare the computing performance with CPUs and GPUs.<br>
Mentors: Xiangyang Ju (LBNL) and Paolo Calafiura (LBNL)
* **Particle flow reconstruction for current and future detectors.**<br>
Particle flow reconstruction is one example of combining low-level measurements across detectors. Performance is important to allow all of the inputs to be combined in a reasonable amount of time. The work from this project can be relevant for the ATLAS experiment or future experiments.<br>
Mentor: Ben Nachman (SLAC)
* **High-throughput reconstruction/simulation with batched input.**<br>
We typically train inference models with batches of events, but we *evaluate* on single events, one at a time. This project would explore the possibility of batch processing on the evaluation side, providing an alternative to the parallel processing event model.<br>
Mentor: Ben Nachman (SLAC)
* **Vectorized particle tracking algorithms.**<br>
Better track finding algorithms allow for a higher quantity and quality of correctly identified displaced tracks, enabling us to investigate interesting processes, such as those involving Higgs bosons and other new particle candidates.
This project uses Line Segment Tracking inputs for GNN studies with the CMS experiment,
systematically determining how ML solutions compare to existing algorithms in performance.
<br>
*Trainee: Jade Chismar (UCSD). Mentor: Giuseppe Cerati (FNAL).*
* **Foundational models for high-energy physics.**<br>
Foundational models in machine learning serve as versatile starting points for tackling
a variety of related but distinct tasks.
This project creates a pre-trained model and uses transfer learning for specific downstream tasks.
The benchmarks are event classification and electron/photon reconstruction with the ATLAS detector.
<br>
*Trainee: Charlie Hultquist (UCB). Mentors: Steven Farrell (LBNL) and Xiangyang Ju (LBNL).*
* **Data Augmentation for Machine Learning.**<br>
The newest generation of flavor tagging algorithms utilize Graph Neural Networks
(GNN), machine learning models which represent jets as fully connected graphs with individual charged
particle tracks as nodes.
When these networks suffer from overtraining, the input datasets can be artificially
expanded to create training samples that better reflect data.
<br>
*Trainee: Hadley Santana Queiroz (UCB). Mentor: Paolo Calafiura (LBNL).*
* **Unfolding Experimental Distributions at Scale.**<br>
Unfolding is one of the main computational tasks across HEP to measure differential cross sections. The purpose of this project is to expand the capabilities and scalability of the OmniFold algorithm by using the Perlmutter supercomputer as a platform. This will require implementation of multi-GPU support using distributed data parallelism and support for multiple frameworks.
*Trainee: Abdelrahman Elabd (UW). Mentor: Wahid Bhimji (LBNL).*
* **Event Filter Tracking and Track Building Optimization.**<br>
We will see an increase in data generation rates and complexity per event with the upgraded
HL-LHC. New tracking algorithms that require fewer computational resources will need to be developed to run at the trigger level. The most expensive stage of the pipeline is the graph segmentation which produces track candidates. This project will optimize and rewrite the connected components and walkthrough algorithms, using junction removal to improve performance.<br>
*Trainee: Levi Condren (UCI). Mentors: Xiangyang Ju (LBNL) and Daniel Murnane (LBNL).*

[jekyll-organization]: https://github.com/watchep

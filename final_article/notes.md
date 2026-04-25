# Notes for Paper
## Platform incompatibility

> In practice, the bottleneck of our method will lie in writing a fast numerical solver that is also compatible with the differentiation procedure of the machine learning package used

So we are currently manually implementing the loss differentiation function since CUDA sPEGG and NumPy are not compatible with PyTorch vectors / matrices.

$\rightarrow$ We might implement a CUDA code that effectively iterates over different network nodes / simulation parameters in parallel.

# Paper skeleton
## Abstract

A quick overview and rundown of the paper.

## Introduction

- Define sPEGG, **cite sPEGG paper**
    - 1 to 2 sentences to highlight some achievements with sPEGG **cite sPEGG and PVA papers**
- Recurring problem: Abundant field evolutionary database, want to learn the evolutionary dynamic patterns
    - sPEGG model involves simulation parameters
    - It'd be nice to predict / estimate those parameters that drive evolution dynamics in the direction observed in such field data.
    - Cite: **Caiman paper**, **PVA paper**, ...
    - Pivot to Neural Network
        - Autodifferentiation feature
        - Parallel computing
        - Might use this to estimate the simulation parameters
- Question: Can we, and to what extend, can we estimate the parameters using differentiation feature of the NN?

## Objective

- Introduce NeuralABM tool
    - Developed by who? **cite**
    - Briefly introduce some pipelines built using NeuralABM **cite**
    - What it can do? Briefly explain how the tool works (i.e. Infrastructure to build NN model for ABM Simulation models)
- Want to integrate NeuralABM pipeline with sPEGG to see if we can predict locus-specific recombination rates
    - When no genes favor reproduction
    - When a gene favors reproduction

## Methodology
## Results
## Discussion


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

## Revision
- Biological implication of the software / program
- Two types of sciences
    1. Target concrete problem - basic science - blue sky
        - Blue skies science
        - Open ended - try to understand the world
        - I.e. Astronomy - does not change anything in real life, but enhance knowledge. Does not matter if we solve anything, we just want to know about the world.
    2. Applied science - THE PAPAER IS WIRED IN THIS WAY
        - Engineering -> impact
        - Conservation, healthcare, medicine
    3. Basic science
        - Does it really MATTER to know the evolution dynamics of the animals?
    => WE ARE LOOKING FROM THE PERSPECTIVE OF BASIC SCIENCE!

- 2 sections: INTRODUCTION & IMPLICATIONS

- Why would biologists have to care about our results? GIVE IT SOME THOUGHTS
    - Even if climate change stops, why is this research still crucial?
    - Why do non-specialists still have interest in our work?

- Antagonistic Pleiotropy (In Aging): based on a single gene -> trade-off in different phenotypes.
    - Endurance vs. Speed
    - Aging: Reproductivity vs. Life span
    - Our model: Mortality vs. Reproductive potential.

    - ADD: Convergence of the reproduction rate


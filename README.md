# Thompson Sampling for Linearly Constrained Bandits

## Overview
This repository contains the code for running the simulations and generating the plots reported in the following paper:  

Saxena V., Gonzalez J.E., Jaldén J., Thompson Samplingh for Linearly Constrained Bandits, AISTATS 2020, Palmerno, Italy.

The code simulates two algorithms: LinConTS and LinCon-KL-UCB. Details and pseudocode of the algorithms are available in the paper. Two real-world datasets are considered, which are included under the datasets/ directory and are also available for download here:  
1. [Coupon-purchase](https://www.kaggle.com/c/coupon-purchase-prediction/data)
2. [edX-course](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2889436)

## Dependencies
The code runs on Jupyter Notebook running a Python3 kernel. Further, the code depeds on the following libraries:  
1. [CVXOPT](https://github.com/cvxopt/cvxopt) for solving a linear program in each step of the algorithm.  
2. [Ray](https://github.com/ray-project/ray) for distributing parallel runs over multiple cores within a compute cluster.  

## Running the Experiments
The experiments can be run by executing each cell in the 'LinConTS_coupon' and 'LinConTS-edX' notebooks. The results are stored to the disk as Numpy arrays.

## Plotting
The results for each of the simulated datasets are plotted with the 'LinConTS_plots' notebook. Make sure to correctly specify the location of the result dataset (as a Numpy array) in the appropriate cell.

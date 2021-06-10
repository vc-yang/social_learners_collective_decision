# Repository for "When do Social Learners Affect Collective Performance Negatively? The Predictions of a Dynamical-System Model"
This repository contains code for paper "When do Social Learners Affect Collective Performance Negatively? The Predictions of a Dynamical-System Model"

The paper related to this repository can be found on arXiv: [https://arxiv.org/abs/2104.00770](https://arxiv.org/abs/2104.00770). The code in this repository is written in Python 3, and was last successfully ran in June 2021 using Python 3.7 in Jupyter Labs. Authored by Vicky Chuqiao Yang and Harvey McGuinness. Last updated in June 2021. 

`Well-mixed model solve odes.ipynb` simulates the baseline model described the paper. It runs the differential equation system in the paper and performs analysis of the fixed points and their stability. 

`my_functions.ipynb` contains core functions which are called for in multiple scripts. These functions are: 

`Two-D grid simulation.ipynb` models a network of nodes via the creation of two matrices. Matrix A corresponds to the opinion state of each node, while Matrix B corresponds to the learning behaviour each node on the network uses (i.e. individual vs social). Matrix A updates to reflect changes in opinion at each time step, while Matrix B is static. Individual learners update from opinion X to Y with a probability m at each time step, while they update from Y to X with probability 1-m. Social learners index the opinion of their four neighbors on the network, then update based upon the proportion of their neighbors holding opinion 0. Updating ceases once the network converges, which is defined via the checkConverge function.

`Gradient learner model.ipynb` simulates the extension of the model where each individual is on a spectrum of social and individual learning. 

`Well mixed model with strength.ipynb` simulates the opinion strength extension, which considers individual learners can hold opinions $X$ and $Y$ with different strength or "stubborness". 

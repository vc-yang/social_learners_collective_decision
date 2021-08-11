# Repository for "Dynamical-System Model Predicts When Social Learners Impair Collective Performance"
This repository contains code for paper "Dynamical-System Model Predicts When Social Learners Impair Collective Performance"

The paper related to this repository can be found on arXiv: [https://arxiv.org/abs/2104.00770](https://arxiv.org/abs/2104.00770). The code in this repository is written in Python 3, and was last successfully ran in June 2021 using Python 3.7 in Jupyter Labs. Authored by Vicky Chuqiao Yang and Harvey McGuinness. Last updated in June 2021. 

`baseline_model.ipynb` analyzs the baseline model described the paper. It runs the differential equation system in the paper and performs analysis of the fixed points and their stability. This script produces Fig 2 of the main text, and Fig S1 of the supplement. 

`spectrum_extension.ipynb` simulates the extension of the model where each individual is on a spectrum of social and individual learning (SM 5.1). 

`spatial_extension.ipynb` simulates the system where individuals are placed on a 2D grid and social learners are only affected by their immediate neighbors (SM 5.2)

`noise_extension.ipynb` simulates the extension of model where noise is added to the system (SM 5.3)

`opinion_strength_extension.ipynb` simulates the opinion strength extension model (SM 5.4), which considers individual learners can hold opinions $X$ and $Y$ with different strength or "stubborness". 

`my_functions.ipynb` contains core functions which are called for in multiple scripts.




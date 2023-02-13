# Learning of discrete Lagrangian densities from data
Accompanying source code for the conference paper

	Learning discrete Lagrangians for variational PDEs from data and detection of travelling waves
	Christian Offen, Sina Ober-Blöbaum
	Conference Proceedings of GSI'23 6th International Conference on Geometric Science of Information (30/08-01/09/2023)
	Saint-Malo, Palais du Grand Large, France
	arXiv: https://arxiv.org/a/offen_c_1.html
	Status: Submitted.

# Main files
	
## FitDensity.jl
The scripts creates training data of a discrete field theory (discrete wave equation). Based on the training data it learns a model of discrete Lagrangian density.

## Evaluation_Trained_Model.ipynb
Jupyter notebook containing numerical experiments with a machine learned discrete density on data of the discrete wave equation. Prediction accuracy is assessed and travelling waves are detected and compared to a reference.


# Supporting files

## 7ptStencilFun.jl
Variational integrator for 1st order discrete field theories (2 dimensional space-time) and tools for preformance evaluation.

## SpectralTools.jl
Tools for spectral interpolation and computation of spectral derivatives on periodic spatial domains.

## TrainingData.jl
Creation of training data to be used in FitDensity.jl

## 2023-01-31_08-53-14run_data.json
Learned model of a Lagrangian density. Created by FitDensity.jl

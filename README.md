# Shimming with the target field approach
A shimming algorithm for Halbach-based low-field magnetic resonance magnets calculating the placement of permanent magnets to compensate field inhomogeneities. The shim strategy is based on placing individual permanent magnet around the bore. The algorithm is a genetic algorithms based on `python` and the `deap` module, which determine the placement of the shim magnets and their orientation. The algorithm only considers the *z*-component of the magnetic flux and the distributions of the individual magnets are estimated with the dipole approximation. The field representation is the target field approach.

## Getting started
The main file is the jupyter-notebook `ShimmingSimulation.ipynb`, which step by step walks you through the logic of the algorithm. The file `shimmingFunctions.py` is containing all the functions needed by the main file and needs to be in the same folder as the main file. 

For some preliminary tests you can set the population size to 250, minGeneration to 40 and maxGeneration to 40. The algorithm will be far from converged, however, you can test if it does what you think.

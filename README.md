# moe_dse

This package provides an automated framework to enable efficient FPGA acceleration of MoE models, by afinding the hardware implementation of expert computations with low latency, under resource constraints. We propose an algorithm to iteratively search for optimal or feasible solutions with an ILP formulation, successively relaxing constraints in each iteration. The detailed steps to run this framework, and associated folders are as follows:

./IP: The folder which generates the IP candidates for DSE, and the associated characterics

./switch-base-8: The folder which generates expert token distribution for MoE, for DSE and validation

./moe\_model: The scripts to conduct DSE, and generate final solution and its associated implmentations

Please refer to README.md in each folder for command line.

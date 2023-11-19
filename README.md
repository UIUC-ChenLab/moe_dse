# moe_dse

This package provides an automated framework to enable efficient FPGA acceleration of MoE models, by finding the hardware implementation of expert computations with low latency, under resource constraints. It runs an algorithm to iteratively search for optimal or feasible solutions with an ILP formulation, successively relaxing constraints in each iteration. The output is the HLS C++ for the selected MoE implementation system for the target FPGA. The detailed steps to run this framework, and associated folders are as follows:

* step1: Generate the IP candidates for DSE, and the associated characteric models. Detailed steps are scripts are in folder ./IP.

* Step2: Generate expert token distribution for MoE, for DSE and validation. Detailed steps and scripts are in folder ./switch-base-8.

* Step3: Conduct DSE, and generate final solution and its associated implmentations. Detailed steps and scripts are in folder ./moe\_model.

# DriverRegulators
Identify transcription factors underlying cell state transitions in scRNAseq datasets

This repository contains the source code and information regarding the DriverRegulators pipeline (Grimaldi et al. 2021).

## Workflow

This python code combines the output of 2 python libraries, pyscenic and scvelo, into a network of transcription factors and associated target genes.
The general workflow is:

1-Running scvelo and saving the top driver genes by cluster as a table

2-Running pyscenic on the same dataset and generating the "f_loom_final.loom" file

3-Using the DriverRegulators code to generate a table of nodes and edges

4-Using a program such as Gephi to visualize the network


# DriverRegulators
Identify transcription factors underlying cell state transitions in scRNAseq datasets

This repository contains the source code and information regarding the DriverRegulators pipeline (Grimaldi et al. 2021).

## Workflow

This python-based code combines the output of 2 python libraries, pyscenic and scvelo, into a network of transcription factors and associated target genes.
The general workflow is:

1-Running scvelo and saving the top driver genes by cluster as a table

2-Extracting the AUC matrix and the regulons from the f_final.loom file of pyscenic output

3-Generate tables of Nodes and Edges based on interactions found in a given cluster

4-Using a program such as Gephi to visualize the network


# DriverRegulators
Identify transcription factors underlying cell state transitions in scRNAseq datasets

This repository contains the source code and information regarding the DriverRegulators pipeline (Grimaldi et al. 2021).

# Workflow

This python code combines the output of 2 python libraries, pyscenic and scvelo, into a network of transcription factors and associated target genes.
The general workflow is:
-Running scvelo and saving the top driver genes by cluster as a table
-Running pyscenic on the same dataset and generating the "f_loom_final.loom" file
-Using the DriverRegulators code to generate a table of nodes and edges
-Using a program like Gephi to visualize the network


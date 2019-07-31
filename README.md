# Human-CyTOF-paper1
Raw data and analysis of CyTOF experiments - first human paper

This repository includes the raw data and core R script that will replicate Figures 1E, 1G, 1H, and Supplementary Figure 1D in the human pancreatic cancer immunoprofiling paper. 

There are four separate Excel and CSV files containing information used by the R script to organize, label, and analyze the data:
1. "sample metadata" - this file contains the file names, associated sample IDs, tissue type (normal versus cancer), dates and batches of sample acquisition
2. "analyzed markers" - this is the selected list of CyTOF parameters used by the R script within the FCS files to perform the entire analysis including clustering and population identification.
3. "labels" - this file contains common labels used by the R script to label all CyTOF parameters within each file with common labels to allow appropriate subsequent loading and analysis by the R script.
4. "cluster merging" - this file contains the final expert-curated set of immune population assignments for the subpopulations initially identified by the ConsensusClusterPlus package.

To replicate the analysis, place the R script and the four files in the same root directory. The FCS files should be placed in a "raw data" folder in the same root directory. This mirrors the organization of this repository. The R script will then run and generate the four figures found in the manuscript.

- Fil Bednar
- July 31, 2019

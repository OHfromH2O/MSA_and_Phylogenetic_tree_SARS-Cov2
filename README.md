# 🦠 SARS-CoV-2 Multiple Sequence Alignment (MSA) & Phylogenetic Analysis
**Computational Biology Lab Assignment**

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.x-blue.svg)
![Biopython](https://img.shields.io/badge/library-Biopython-orange.svg)

## 📌 Overview
This repository contains a **Multiple Sequence Alignment (MSA) and Phylogenetic Tree Construction project** for SARS-CoV-2 genomic (or protein) sequences, conducted as part of a Computational Biology lab assignment.

The primary goal of this project is to comparatively analyze SARS-CoV-2 sequences collected from various regions and timeframes, in order to structurally visualize their evolutionary relationships and key mutation patterns.

## 🎯 Objectives
1. **Sequence Preprocessing:** Collect and clean SARS-CoV-2 sequences (FASTA format) from databases such as NCBI or GISAID.
2. **Multiple Sequence Alignment (MSA):** Identify conserved regions and mutation sites across sequences through homology comparison.
3. **Phylogenetic Analysis:** Calculate evolutionary distances based on the aligned sequences to construct and visualize phylogenetic trees, analyzing the relationships between different clades.

## 🛠️ Methods & Tools
> 💡 *Note: Please keep only the tools you actually used during the lab and delete/modify the rest.*
* **Data Sources:** [NCBI Virus / GISAID]
* **MSA Tools:** [Clustal Omega / MAFFT / MUSCLE]
* **Phylogenetic Algorithms:** [Neighbor-Joining (NJ) / Maximum Likelihood (ML)] (Tools used: MEGA / IQ-TREE / FastTree, etc.)
* **Visualization Tools:** [FigTree / iTOL (Interactive Tree Of Life) / Python (Matplotlib, Biopython)]
* **Programming Language:** [Python / R / Bash]

## 📁 Repository Structure
```text
MSA_and_Phylogenetic_tree_SARS-Cov2/
│
├── data/                  # Raw and preprocessed FASTA sequence data
│   ├── raw_sequences/     # Original files downloaded from NCBI/GISAID
│   └── aligned_data/      # Processed files after MSA (.aln, .fasta)
│
├── scripts/               # Python/R scripts used for analysis
│   ├── 01_data_prep.py    # Data preprocessing script
│   ├── 02_run_MSA.py      # Script to execute sequence alignment
│   └── 03_build_tree.py   # Script for tree construction and visualization
│
├── results/               # Final outputs and visualization images
│   ├── phylogenetic_tree.png  # Rendered phylogenetic tree image
│   └── tree_file.nwk          # Newick tree file for visualization tools
│
└── README.md              # Project documentation
📊 Key Results
(Summarize your core findings or insights here. Attaching an image of your phylogenetic tree is highly recommended!)

Phylogenetic Tree Visualization: <img src="results/phylogenetic_tree.png" width="600" alt="SARS-CoV-2 Phylogenetic Tree">

Analysis Summary: * The analysis confirmed that specific variants (e.g., Omicron, Delta) form distinct clades diverging from the original sequences.

Concentrated mutations were particularly observed near the Spike protein sequence regions.

🚀 Usage
To reproduce this project in your local environment, follow these steps:

1. Clone the repository

Bash
git clone [https://github.com/OHfromH2O/MSA_and_Phylogenetic_tree_SARS-Cov2.git](https://github.com/OHfromH2O/MSA_and_Phylogenetic_tree_SARS-Cov2.git)
cd MSA_and_Phylogenetic_tree_SARS-Cov2
2. Install required packages

Bash
pip install biopython matplotlib pandas
3. Run the scripts

Bash
# Data preprocessing and MSA execution
python scripts/02_run_MSA.py

# Phylogenetic tree construction
python scripts/03_build_tree.py
👨‍💻 Author
GitHub: @OHfromH2O

Course: [KUL, Computational Biology Lab, Autumn 2023]

This assignment was conducted to understand and apply evolutionary analysis pipelines using computational biology techniques.

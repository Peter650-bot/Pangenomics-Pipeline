# Pangenomic Automated Workflow

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Output](#output)
- [Limitations](#limitations)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)
- [References](#references)
- [Contact](#contact)

## Overview
This project provides an automated pipeline for pangenomic analysis of bacterial strains. The workflow processes genomic data to:
- Extract coding sequences (CDS)
- Cluster homologous genes
- Classify genes into core/accessory/unique categories
- Perform functional annotation
- Generate visualizations

Key improvement: Supports novel sequences not in PATRIC database.

## Features
- **Flexible Input**: Works with both PATRIC IDs and user-provided FASTA files
- **Automated Analysis**: Single script execution
- **Comprehensive Outputs**:
  - Gene clusters
  - Functional annotations (COG/GO terms)
  - Statistical analysis
  - Visualization plots
- **Translation Function**: Automatically converts DNA CDS to protein for annotation

## Installation

### Requirements
- Python 3.6+
- Linux environment (tested on Ubuntu 20.04)

### Dependencies
```bash
# Python libraries
pip install pandas numpy scipy matplotlib biopython

# External tools
sudo apt-get install cd-hit
sudo apt-get install eggnog-mapper

# Configure tools

export PATH=$PATH:/path/to/eggnog-mapper
source ~/.bashrc

export PATH=$PATH:/path/to/cd-hit
source ~/.bashrc

# Activate and run workflow1.sh
chmod +x workflow1.sh
./workflow1.sh


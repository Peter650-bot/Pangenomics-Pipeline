# Pangenomic Automated Workflow

## Table of Contents
- [Overview](#overview)
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
- Cluster homologous genes
- Classify genes into core/accessory/unique categories
- Perform functional annotation
- Generate visualizations

## Installation

### Requirements
- Python 3.6+
- Linux environment (tested on Ubuntu 20.04)
  
### Dependencies
Make sure to install these dependencies before proceeding.
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


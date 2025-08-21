Salmonella AMR Project
Practice started 2025-08-19
=======
# Salmonella_amr
I am learning the linux and bioinformatics by reproducing nature article 
named A global atlas and drivers of antimicrobial resistance in Salmonella during 1900-2023 

paper DOI
## https://doi.org/10.1038/s41467-025-59758-3
>>>>>>> origin/main

how to create the folder directroy

# Salmonella-AMR: Global Atlas of Antimicrobial Resistance in Salmonella (1900–2023)

## 📌 Project Overview
This project aims to reproduce and extend analyses from  
**"A global atlas and drivers of antimicrobial resistance in Salmonella during 1900–2023"**  
by collecting public genomes, identifying antimicrobial resistance (AMR) genes,  
and linking genomic data with metadata (country, year, serovar, host, antibiotic use).

---

## 📂 Project Structure

salmonella-amr/
├── config/ # configuration files (e.g., snakemake config.yaml, tool params)
├── data/
│ ├── raw/ # raw downloaded data (NCBI SRA, ENA, GISAID if allowed)
│ ├── processed/ # cleaned/parsed metadata and intermediate data
│ └── external/ # external reference DBs (CARD, ResFinder, WHO surveillance data)
├── scripts/ # Python, R, Bash scripts
├── notebooks/ # Jupyter notebooks / exploratory analyses
├── results/
│ ├── qc/ # fastqc, multiqc reports
│ ├── alignment/ # reference-based alignments
│ ├── variants/ # variant calls (if used)
│ ├── amr/ # AMR gene detection results
│ ├── metadata/ # curated metadata tables (country/year/serovar/host)
│ └── figures/ # final plots, maps, charts
├── logs/ # pipeline logs
├── tmp/ # temporary files (ignored in git)
└── analysis/ # workflow files (Snakemake, Nextflow)

```
$ mkdir -p salmonella-amr/{config,data/{raw,processed,external},\
scripts,notebooks,results/{qc,variants,alignment,figures,amr,metadata},\
logs,tmp,analysis}

```
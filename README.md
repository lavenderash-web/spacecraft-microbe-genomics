# Comparative Genomics of Heat-Shock-Tolerant Microbes Isolated from a Spacecraft Assembly Facility

## Project Overview

This project investigates the genomic characteristics and evolutionary relationships of 63 heat-shock-tolerant microbial isolates obtained from a spacecraft assembly facility.

The study focuses on genome quality assessment, genome annotation, functional characterization, pangenome analysis, and phylogenetic relationships to better understand the genomic diversity of these microorganisms.

The isolates were selected based on their ability to survive heat shock at 80°C for 15 minutes.

## Research Objectives

- Assess the quality and completeness of microbial genome assemblies.
- Annotate genomes and predict protein-coding genes.
- Characterize predicted proteins and their functional annotations.
- Investigate shared and accessory gene families through pangenome analysis.
- Identify core genes and explore evolutionary relationships among isolates.
- Develop a reproducible bioinformatics workflow for comparative genomics.

## Dataset

- **Number of isolates:** 63
- **Source:** Spacecraft assembly facility
- **Heat-shock condition:** 80°C for 15 minutes
- **NCBI BioProject:** [PRJNA728748](https://www.ncbi.nlm.nih.gov/bioproject/PRJNA728748)
- **Data type:** Publicly available microbial sequencing reads and genome assemblies

## Bioinformatics Workflow

### 1. Raw Read Quality Control and Preprocessing
Tools: FastQC, Trimmomatic / Cutadapt

Assess sequencing quality and perform read trimming and adapter removal where required.

### 2. Genome Assembly
Tool: SPAdes

Generate draft genome assemblies from sequencing reads.

### 3. Genome Assembly Quality Assessment
Tools: QUAST, CheckM

Evaluate assembly statistics, including genome size, contig count, N50, GC content, estimated completeness, and contamination.

### 4. Genome Annotation
Tool: Prokka

Predict genomic features, including coding sequences and proteins, and generate standardized genome annotations.

### 5. Functional Annotation
Tool: eggNOG-mapper

Characterize predicted proteins using functional annotations, including COG categories and available pathway information.

### 6. Pangenome Analysis
Tool: Panaroo

Investigate gene-family distribution across isolates and characterize core, soft-core, shell, and cloud gene families.

**Status:** In progress.

### 7. Core-Genome Phylogenetics
Tools: MAFFT, IQ-TREE

Develop a core-genome alignment and infer phylogenetic relationships among the isolates.

**Status:** In progress.

## Tools and Technologies

- **Languages:** Python, R (where applicable)
- **Quality control:** FastQC
- **Read preprocessing:** Trimmomatic, Cutadapt
- **Genome assembly:** SPAdes
- **Assembly assessment:** QUAST
- **Genome quality assessment:** CheckM
- **Genome annotation:** Prokka
- **Functional annotation:** eggNOG-mapper
- **Pangenome analysis:** Panaroo
- **Sequence alignment:** MAFFT
- **Phylogenetic inference:** IQ-TREE
- **Workflow environment:** Galaxy Europe and command-line tools

## Repository Structure

```text
spacecraft-microbe-comparative-genomics/
├── README.md
├── scripts/
├── genome_quality/
├── annotation/
├── pangenome/
├── phylogenetics/
└── results/
```

Directories will be populated with relevant scripts, documentation, summary tables, and figures as the project progresses.

## Project Status

Genome assembly, quality assessment, and annotation workflows have been undertaken. Functional annotation and comparative analyses are being integrated into the project, with pangenome analysis and core-genome phylogenetics ongoing.

Only validated outputs will be added as final results.

## Reproducibility

The repository will document the tools, parameters, input data sources, and analysis steps used throughout the workflow. Public accession numbers will be provided where applicable to support reproducibility.

## Acknowledgements

The sequencing data originate from the publicly available study, *Draft Genome Sequences of Heat Shock-Tolerant Microbes Isolated from a Spacecraft Assembly Facility*.

This repository documents an independent bioinformatics analysis of publicly available genomic data.

## License

See the repository license for the terms governing reuse of the original code and documentation. Original sequencing data and third-party resources remain subject to their respective terms.

# Comparative Sequence Homology and Evolutionary Conservation Analysis of VEGFR2

## Project Overview

This project presents a bioinformatics workflow for investigating the evolutionary conservation and structural homology of **Vascular Endothelial Growth Factor Receptor 2 (VEGFR2/KDR)** across three commonly used mammalian species: **Human (*Homo sapiens*)**, **Mouse (*Mus musculus*)**, and **Rat (*Rattus norvegicus*)**.

The study combines **Python-based sequence retrieval, BLASTp homology analysis, Multiple Sequence Alignment (MSA), conservation heatmap generation, and Power BI analytics** to evaluate the suitability of rodent models for translational VEGFR2-targeted drug discovery research.

---

## Research Objective

To assess the degree of sequence conservation and functional domain preservation of VEGFR2 across human, mouse, and rat proteins, thereby validating the biological relevance of rodent models in preclinical anti-cancer drug development.

---

## Tools & Technologies

### Programming & Automation

* Python 3
* Jupyter Notebook
* Biopython (Entrez API)

### Bioinformatics Tools

* NCBI Protein Database
* NCBI BLASTp
* Clustal Omega

### Data Analytics & Visualization

* Power BI
* Matplotlib
* Seaborn
* Microsoft Excel

---

## Workflow

### 1. Automated Sequence Retrieval

A Python-based pipeline was developed using Biopython's Entrez module to automatically retrieve VEGFR2 protein sequences from the NCBI Protein database.

#### Protein Accessions

| Species           | Accession ID   |
| ----------------- | -------------- |
| Homo sapiens      | NP_002244.1    |
| Mus musculus      | NP_001390070.1 |
| Rattus norvegicus | NP_037194.2    |

### Output

* FASTA sequence files generated automatically.
* Standardized datasets prepared for downstream analysis.

---

### 2. Cross-Species Homology Analysis using BLASTp

Human VEGFR2 was used as the reference sequence and compared against mouse and rat orthologs using BLASTp.

The analysis focused on:

* Sequence identity
* Query coverage
* Conserved functional domains
* Active-site residue preservation

### Key Findings

| Comparison     | Sequence Identity | Query Coverage |
| -------------- | ----------------- | -------------- |
| Human vs Mouse | 85.79%            | 100%           |
| Human vs Rat   | 86.92%            | 93%            |

### Conserved Functional Regions

The following critical domains remained highly conserved:

* PTKc_VEGFR2 catalytic kinase domain
* ATP-binding pocket
* Immunoglobulin-like extracellular domains
* Activation loop residues
* Catalytic active-site regions

---

### 3. Multiple Sequence Alignment (MSA)

A comprehensive Clustal Omega Multiple Sequence Alignment was performed to identify residue-level conservation across all three species.

Alignment symbols were interpreted as:

| Symbol | Meaning                         |
| ------ | ------------------------------- |
| *      | Complete residue conservation   |
| :      | Strongly conserved substitution |
| .      | Weakly conserved substitution   |

### Analysis Goals

* Detect evolutionary mutations
* Identify conserved motifs
* Examine residue-level divergence
* Evaluate structural stability of functional domains

---

### 4. Conservation Heatmap Generation using Python

A custom Python workflow was developed to process alignment outputs and generate sequence conservation heatmaps.

### Visualization Features

* Residue conservation scoring
* Comparative species mapping
* High-conservation region detection
* Functional domain highlighting

### Libraries Used

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

---

### 5. Interactive Power BI Analytics Dashboard

Alignment statistics and BLAST metrics were integrated into a Power BI dashboard to provide interactive comparative analysis.

### Dashboard Metrics

* Sequence identity percentages
* Query coverage
* Species-wise conservation profiles
* Evolutionary divergence indicators
* Functional domain preservation summaries

---

## Biological Significance

Rodent models are extensively used during preclinical oncology studies. Therefore, validating target conservation between humans and model organisms is essential before advancing candidate therapeutics.

The analysis demonstrated:

* Greater than 85% sequence identity across species.
* Near-complete query coverage.
* Strong conservation within the ATP-binding pocket and kinase catalytic domains.

These findings support the translational relevance of mouse and rat models for evaluating VEGFR2-targeting phytochemical inhibitors identified during virtual screening studies.

---

## Key Skills Demonstrated

### Bioinformatics

* Comparative genomics
* Sequence homology analysis
* Multiple sequence alignment
* Evolutionary conservation studies
* Functional domain analysis

### Programming

* Python automation
* API-based biological data retrieval
* Data preprocessing
* Scientific computing

### Data Analytics

* Data visualization
* Dashboard development
* Biological data interpretation
* Scientific reporting

### Tools

* Python
* Biopython
* BLASTp
* Clustal Omega
* Power BI
* Excel
* Matplotlib
* Seaborn

---

## Repository Structure

| File                           | Description                                      |
| ------------------------------ | ------------------------------------------------ |
| README.md                      | Complete project documentation                   |
| data_retrieval_from_NCBI.ipynb | Python pipeline for automated sequence retrieval |
| MSA_heatmap_generation.ipynb   | Heatmap generation workflow                      |
| human_vegfr2.fasta             | Human VEGFR2 sequence                            |
| mouse_vegfr2.fasta             | Mouse VEGFR2 sequence                            |
| rat_vegfr2.fasta               | Rat VEGFR2 sequence                              |
| blastp_results_dashboard.pbix  | Power BI dashboard                               |
| BLAST_RESULT_SS.png            | Dashboard visualization                          |
| blastp_screenshot.png          | Functional domain alignment output               |
| MSA_RESULT.png                 | Clustal Omega alignment result                   |
| vegfr2_msa_heatmap.png         | Conservation heatmap generated using Python      |

---

## Project Outcome

This project successfully integrated **Python programming, bioinformatics analysis, and data analytics** to evaluate VEGFR2 conservation across clinically relevant mammalian species. The results demonstrated strong evolutionary preservation of critical functional domains, supporting the use of rodent models in VEGFR2-focused anti-cancer drug discovery and translational research.

---

## Author

**Shreya Upadhyay**

Aspiring Bioinformatics & Healthcare Data Analyst

**Skills:** Python | SQL | Power BI | Excel | Bioinformatics | Comparative Genomics | Data Visualization | Molecular Docking


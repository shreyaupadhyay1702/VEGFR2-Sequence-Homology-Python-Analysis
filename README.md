# Comparative Sequence Homology and Evolutionary Conservation Analysis of VEGFR2

A Python-driven bioinformatics pipeline designed to programmatically fetch, align, and analyze the sequence conservation and domain architecture of Vascular Endothelial Growth Factor Receptor 2 (VEGFR2) across Human (*Homo sapiens*), Rat (*Rattus norvegicus*), and Mouse (*Mus musculus*).

---

## 📌 Project Overview
Understanding structural conservation in therapeutic targets across model organisms is crucial for translational drug discovery. This project automates the retrieval of VEGFR2 protein sequences using Python, performs comparative homology analysis via web-based and local tools (NCBI BLASTp and ClustalOmega MSA), identifies highly conserved active domains, and maps the results using custom Matplotlib heatmaps and interactive Power BI analytics dashboards.

---

## 🛠️ Tech Stack & Tools
* **Programming & Automation:** Python 3 (Jupyter Notebook), Biopython (Entrez/NCBI API)
* **Bioinformatics Algorithms:** NCBI BLASTp, ClustalOmega (Multiple Sequence Alignment)
* **Data Visualization & Analytics:** Power BI, Matplotlib / Seaborn (for Conservation Heatmaps)

---

## 🚀 Workflow Architecture

### 1. Automated Sequence Retrieval (Python)
* Developed a Jupyter Notebook pipeline utilizing NCBI Entrez utilities to programmatically fetch VEGFR2 protein sequences in FASTA format using targeted database Accession IDs:
  * **Human (*Homo sapiens*):** `NP_002244.1`
  * **Mouse (*Mus musculus*):** `NP_001390070.1`
  * **Rat (*Rattus norvegicus*):** `NP_037194.2`

### 2. Sequence Homology Analysis (BLASTp)
* Conducted **BLASTp** alignments to cross-reference multi-species sequence uniformity against the human query structure.
* Mapped crucial domain architectures, pinpointing the **PTKc_VEGFR2** (Protein Tyrosine Kinase catalytic domain), **Ig-like** structural blocks, active site residue sequences, and the central ATP-binding pocket.
* **Key Homology Findings:**
  * *Human vs Mouse:* 85.79% Sequence Identity, 100% Query Coverage.
  * *Human vs Rat:* 86.92% Sequence Identity, 93% Query Coverage.

### 3. Multiple Sequence Alignment (MSA)
* Executed a full-scale **ClustalOmega** multiple sequence alignment to study exact point mutations and point-to-point residue mutations across the target organisms.
* Analyzed the structural positions to clearly track absolute identity (`*`), highly conserved blocks (`:`), and semi-conserved amino acid substitutions (`.`).

### 4. Data Visualization & Python Heatmaps
* Programmed a custom **Matplotlib/Seaborn** automation script to parse the alignment matrix scores and render clear, data-driven Sequence Identity Heatmaps for fast residue conservation screening.

### 5. Business Intelligence Dashboarding & Translational Insights
* Integrated the multi-species alignment metrics into an interactive **Power BI Dashboard** to dynamically report query coverages, identity ratios, and evolutionary divergence profiles.
* **Translational Significance (In Vivo Pre-clinical Models):** Since rodent models (Mouse/Rat) are universally deployed as primary in vivo surrogates for oncology drug testing, validating target homology is non-negotiable. 
* **Structural Conclusion:** Our alignment recorded extreme conservation (>85% identity and near 100% query coverage) specifically across the critical ATP-binding loops and catalytic active centers. This high sequence preservation mathematically justifies the usage of murine models for evaluating the pharmacodynamics of these newly screened VEGFR2 phytochemical inhibitors before moving to human applications.

---

## 📂 Repository Files List
* **README.md** → Complete project documentation and translational research insights.
* **data retrieval from NCBI.ipynb** → Jupyter Notebook containing the Python pipeline for automated NCBI sequence retrieval via Accession IDs.
* **MSAheatmapgeneration.ipynb** → Custom Jupyter script used to parse alignment scores and plot the sequence identity heatmap using Matplotlib/Seaborn.
* **humanproteinvegfr2.fasta** → Raw FASTA format sequence file for human VEGFR2.
* **mousevegfr2.fasta** → Raw FASTA format sequence file for mouse VEGFR2.
* **ratvegfr2.fasta** → Raw FASTA format sequence file for rat VEGFR2.
* **blastp results analysis.pbix** → Interactive Power BI Dashboard file for cross-species homology analysis and metric tracking.
* **BLAST RESULT SS.png** → High-resolution dashboard output comparing cross-species identity and query coverage.
* **blast p result ss.png** → Secondary graphical plot mapping the multi-species homology analysis.
* **blastp screenshot .png** → Reference graphic showcasing the functional domain architecture and specific hit alignment locations from NCBI BLASTp.
* **MSA RESULT.png** → Output capture of the ClustalOmega multiple sequence alignment showing character-level residue matches.
* **vegfr2_msa_heatmap.png** → The final data-driven identity heatmap exported via the Python visualization script.

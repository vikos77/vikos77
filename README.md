# Vigneshwaran Muthuraman

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vigneshwaran-muthuraman/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vigneshwaran0594@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/vikos77)

---

## Bioinformatics Analyst | NGS Pipeline Development | Antimicrobial Resistance

MSc Bioinformatics (Teesside University, 2025) with 3+ years of clinical laboratory experience spanning molecular diagnostics, antimicrobial resistance research, and microbiome analysis. I build automated pipelines for bacterial genomics and NGS data processing, and I understand the wet-lab context behind the data — having generated a significant portion of it myself.

My work sits at the intersection of computational genomics and applied microbiology: building reproducible workflows, interrogating large-scale genomic datasets, and translating findings into outputs that mean something for AMR surveillance and clinical diagnostics.

> **Open to opportunities** in bioinformatics analysis, NGS pipeline development, and genomics research roles across the UK. [Get in touch.](mailto:vigneshwaran0594@gmail.com)

---

## Projects

### [Acinetobacter Defence System Pipeline](https://github.com/vikos77/acinetobacter-defence-pipeline)
*Production-ready Snakemake workflow for large-scale bacterial defence system analysis*

Acinetobacter baumannii is one of the WHO's priority pathogens — notorious for acquiring resistance and evading clinical interventions — but the relationship between its phage defence systems and antibiotic resistance gene carriage was poorly characterised. I built an end-to-end automated pipeline to investigate this at scale.

**What it does:** Retrieves genomes from NCBI, runs DefenseFinder and PADLOC for defence system prediction, ResFinder for resistance gene identification, and integrative mobile element (IME) prediction — then outputs structured result tables ready for statistical analysis. Fully reproducible across fresh environments.

**Stack:** Snakemake · Python · Bash · DefenseFinder · PADLOC · ResFinder · CRISPRCasFinder

**Scale:** Validated across 500+ *Acinetobacter* genomes

---

### [Acinetobacter Defence Systems — Statistical Analysis](https://github.com/vikos77/Acinetobacter-defence-systems)
*R-based statistical analysis of defence system architecture and AMR correlations*

Companion repository to the pipeline above. Takes the structured output and performs species-level comparative analysis, co-occurrence testing, and correlation mapping between defence system presence, resistance gene load, and mobile genetic element distribution.

**Key finding:** Specific defence systems — particularly Gao_Qat — co-occur with multiple resistance determinants at rates significantly above background, suggesting shared genomic neighbourhoods that may facilitate simultaneous acquisition of defence and resistance. SspBCDE was consistently enriched in *A. baumannii* clinical isolates, implicating it as a factor in this pathogen's clinical persistence.

**Stack:** R · DESeq2 · ggplot2 · Statistical correlation and enrichment analysis

---

### RNA-seq Workflow: R vs Python *(In development)*
*Benchmarking differential expression analysis across two computational stacks*

Most bioinformatics teams have a preferred language for RNA-seq analysis, but the performance and reproducibility differences between DESeq2 (R) and Python-based implementations are rarely documented systematically. This project runs matched datasets through both stacks and documents where results diverge, where they agree, and what drives the differences — aimed at producing a reproducible reference for teams making implementation decisions.

**Stack:** R · DESeq2 · Python · edgeR · Bash

---

## Technical Skills

| Domain | Tools & Technologies |
|--------|---------------------|
| **Pipeline Development** | Snakemake · Bash scripting · Git · reproducible workflow design |
| **NGS Analysis** | FastQC · Trim Galore · BWA · STAR · GATK · SAMtools · QIIME2 |
| **Bacterial Genomics** | DefenseFinder · PADLOC · ResFinder · CRISPRCasFinder · hifiasm |
| **Statistical Analysis** | R (DESeq2, edgeR, ggplot2, Shiny) · Python · SQL |
| **Sequencing Platforms** | Illumina short-read · PacBio HiFi · Oxford Nanopore (library prep and data analysis) |
| **Clinical & Regulatory** | ISO 15189 method validation · GLP · SOP development · high-throughput QC |

---

## Publications

Three peer-reviewed papers spanning COVID-19 diagnostics, antimicrobial resistance, and microbiome analysis:

- **Takke A, Zarekar M, Muthuraman V, et al.** (2022). Comparative study of clinical features and vaccination status in Omicron and non-Omicron infected patients during the 3rd wave in Mumbai. *Journal of Family Medicine and Primary Care*, 11(10), 6135–6142. [DOI](https://doi.org/10.4103/jfmpc.jfmpc_902_22)

- **Daswani P, Muthuraman V, et al.** (2020). Effect of *Psidium guajava* (guava) leaf decoction on antibiotic-resistant clinical diarrhoeagenic isolates of *Shigella* spp. *International Journal of Enteric Pathogens*, 8(4), 122–129. [DOI](https://doi.org/10.34172/ijep.2020.20)

- **Jnana A, Muthuraman V, et al.** (2020). Microbial community distribution and core microbiome in successive wound grades of individuals with diabetic foot ulcers. *Applied and Environmental Microbiology*, 86(6), e02608-19. [DOI](https://doi.org/10.1128/AEM.02608-19)

---

## Background

Before moving into computational work full-time, I spent three years in active research and clinical laboratory environments:

- **ICMR – National Institute of Immunohaematology** — scaled COVID-19 RT-qPCR testing from 100 to 300+ samples/day through workflow automation; built the QC monitoring infrastructure used across the lab's 24/7 operations
- **The Foundation for Medical Research** — AMR research on MDR *Shigella*; designed and validated the 96-well screening assay that underpins the published findings on guava leaf extract
- **Manipal School of Life Sciences** — characterised wound microbiome dynamics in diabetic foot ulcers using 16S rRNA sequencing and QIIME2; the dataset and pipeline from this work were published in *Applied and Environmental Microbiology*

This background shapes how I approach computational problems — I know what the data represents before it enters the pipeline, which changes the questions you ask of it.

---

*MSc Bioinformatics — Teesside University (2025)*
*MSc Molecular Biology & Human Genetics — Manipal University (2017)*

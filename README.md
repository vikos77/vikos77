# Vigneshwaran Muthuraman

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vigneshwaran-muthuraman/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vigneshwaran0594@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/vikos77)

---

## Bioinformatics Analyst | NGS Pipeline Development | Antimicrobial Resistance

Computational biologist and microbiologist with dual MSc qualifications - Bioinformatics with Distinction (Teesside University, 2025) and Molecular Biology and Human Genetics (Manipal University), and a first-author publication in the Journal of Applied Microbiology (2026) on bacterial antiviral defence systems and AMR gene co-evolution across clinical Acinetobacter populations. Four years of active research across pipeline development, population-scale comparative genomics, cancer metagenomics, and high-throughput molecular diagnostics. I build production-grade pipelines for biological problems I understand at bench level.

---

## Projects

### [Acinetobacter Defence System Pipeline](https://github.com/vikos77/acinetobacter-defence-pipeline)
*Production-ready Snakemake workflow for large-scale bacterial defence system analysis*

Acinetobacter baumannii is one of the WHO's priority pathogens - notorious for acquiring resistance and evading clinical interventions, but the relationship between its phage defence systems and antibiotic resistance gene carriage was poorly characterised. I built an end-to-end automated pipeline to investigate this at scale.

**What it does:** Retrieves genomes from NCBI, runs DefenseFinder and PADLOC for defence system prediction, ResFinder for resistance gene identification, and integrative mobile element (IME) prediction then outputs structured result tables ready for statistical analysis. Fully reproducible across fresh environments.

**Stack:** Snakemake · Python · Bash · DefenseFinder · PADLOC · ResFinder · CRISPRCasFinder

**Scale:** Validated across 200+ *Acinetobacter* genomes

**Published:** Findings from this pipeline contributed to a [first-author publication](https://doi.org/10.1093/jambio/lxag069) in *Journal of Applied Microbiology* (2026)

---

### [Acinetobacter Defence Systems — Statistical Analysis](https://github.com/vikos77/Acinetobacter-defence-systems)
*R-based statistical analysis of defence system architecture and AMR correlations*

Companion repository to the pipeline above. Takes the structured output and performs species-level comparative analysis, co-occurrence testing, and correlation mapping between defence system presence, resistance gene load, and mobile genetic element distribution.

**Key finding:** Specific defence systems particularly Gao_Qat co-occur with multiple resistance determinants at rates significantly above background, suggesting shared genomic neighbourhoods that may facilitate simultaneous acquisition of defence and resistance. SspBCDE was consistently enriched in *A. baumannii* clinical isolates, implicating it as a factor in this pathogen's clinical persistence.

**Stack:** R · DESeq2 · ggplot2 · Statistical correlation and enrichment analysis

---

### Long-Read Assembly Workflows: Haploid to Hi-C Phased Diploid
*Reproducible HiFi and HiFi+Hi-C assembly pipelines across three organisms of increasing genomic complexity*

Assembly strategy is not universal - ploidy, heterozygosity, and available data types all determine the right approach. This series of three end-to-end pipelines works through that decision space systematically: a haploid bacterial genome as a clean baseline, a diploid fungal pathogen (*C. albicans*) assembled with HiFi reads only, and a diploid yeast (*S. cerevisiae*) assembled to chromosome level using HiFi + Hi-C phasing data.

The key technical finding: hifiasm's `--primary` mode produces a functional assembly from a diploid genome without phasing data, but the 209 contig output and complex heterozygous bubble graph for *C. albicans* make the limitation tangible. Adding Hi-C chromatin contact maps for *S. cerevisiae* resolves both haplotypes to chromosome-scale 17 and 16 contigs with 0-edge contig graphs and N50 of ~923 kb, demonstrating where HiFi alone is sufficient and where it is not.

**Stack:** hifiasm · seqkit · NanoPlot · FastQC · QUAST · BUSCO (fungi_odb10 · saccharomycetes_odb10) · Bandage

**Repos:** [*E. coli* HiFi](https://github.com/vikos77/ecoli-hifi-assembly) · [*C. albicans* diploid](https://github.com/vikos77/Candida-HIFI-Assembly) · [*S. cerevisiae* Hi-C phased](https://github.com/vikos77/yeast-hifi-hic-assembly)

---

### [16S Amplicon Metagenomics: VSEARCH vs QIIME2](https://github.com/vikos77/metagenomics_wound_microbiome)
*Comparative 16S rRNA pipeline applied to 122 clinical diabetic wound samples*

VSEARCH and QIIME2 are the two dominant tool choices for amplicon-based microbiome analysis, but their performance characteristics on the same clinical dataset are rarely documented directly. This pipeline applies both to 122 diabetic foot ulcer samples from the Jnana et al. (2020) dataset (*Applied and Environmental Microbiology*), quantifying where the methods agree and where they diverge.

Overall community composition shows strong concordance (Pearson r = 0.787 for dominant taxa), but the methods separate substantially on rare organisms wherein VSEARCH detected 820 low-abundance genera against QIIME2's 454, with 322 shared. For clinical microbiome work where rare opportunistic pathogens are relevant, that difference affects what gets reported.

**Stack:** Python · VSEARCH · QIIME2 · DADA2 · BLAST+ (SILVA) · FastQC · Trimmomatic · matplotlib · seaborn

---

## Technical Skills

| Domain | Tools & Technologies |
|--------|---------------------|
| **Pipeline Development** | Snakemake · Bash scripting · Git · reproducible workflow design |
| **NGS Analysis** | FastQC · Trim Galore · BWA · STAR · GATK · SAMtools · QIIME2 |
| **Genome Assembly** | hifiasm (HiFi · Hi-C phased) · Bandage · QUAST · BUSCO |
| **Bacterial Genomics** | DefenseFinder · PADLOC · ResFinder · CRISPRCasFinder |
| **Statistical Analysis** | R (DESeq2, edgeR, ggplot2, Shiny) · Python · SQL |
| **Sequencing Platforms** | Illumina short-read · PacBio HiFi · Oxford Nanopore (library prep and data analysis) |
| **Clinical & Regulatory** | ISO 15189 method validation · GLP · SOP development · high-throughput QC |

---

## Publications

Four peer-reviewed papers spanning genome defence systems, COVID-19 diagnostics, antimicrobial resistance, and microbiome analysis:

- **Muthuraman V, Roy P, Dean P, Lopes BS, Shehreen S.** (2026). The balance between defence systems and horizontal gene transfer shapes adaptation in clinical strains of *Acinetobacter* spp. *Journal of Applied Microbiology*, lxag069. [DOI](https://doi.org/10.1093/jambio/lxag069)

- **Takke A, Zarekar M, Muthuraman V, et al.** (2022). Comparative study of clinical features and vaccination status in Omicron and non-Omicron infected patients during the 3rd wave in Mumbai. *Journal of Family Medicine and Primary Care*, 11(10), 6135–6142. [DOI](https://doi.org/10.4103/jfmpc.jfmpc_902_22)

- **Daswani P, Muthuraman V, et al.** (2020). Effect of *Psidium guajava* (guava) leaf decoction on antibiotic-resistant clinical diarrhoeagenic isolates of *Shigella* spp. *International Journal of Enteric Pathogens*, 8(4), 122–129. [DOI](https://doi.org/10.34172/ijep.2020.20)

- **Jnana A, Muthuraman V, et al.** (2020). Microbial community distribution and core microbiome in successive wound grades of individuals with diabetic foot ulcers. *Applied and Environmental Microbiology*, 86(6), e02608-19. [DOI](https://doi.org/10.1128/AEM.02608-19)

---

## Background

Before moving into computational work full-time, I spent three years in active research and clinical laboratory environments:

- **ICMR – National Institute of Immunohaematology** - scaled COVID-19 RT-qPCR testing from 100 to 400+ samples/day through workflow automation; built the QC monitoring infrastructure used across the lab's 24/7 operations
- **The Foundation for Medical Research** - AMR research on MDR *Shigella*; designed and validated the 96-well screening assay that underpins the published findings on guava leaf extract
- **Manipal School of Life Sciences** - characterised wound microbiome dynamics in diabetic foot ulcers using 16S rRNA sequencing and QIIME2; the dataset and pipeline from this work were published in *Applied and Environmental Microbiology*

This background shapes how I approach computational problems as I know what the data represents before it enters the pipeline, which changes the questions you ask of it.

# Hi, I'm Aswini Leela 👋

**Genomics | Bioinformatics**

I develop and maintain bioinformatics pipelines for whole-genome assembly, metagenomics, and clinical genomics using Oxford Nanopore and PacBio HiFi sequencing technologies.

---

## Research Areas

- Long-read genome assembly (PacBio HiFi, Oxford Nanopore)
- Metagenomics and microbiome analysis
- Clinical genomics and variant calling
- Comparative genomics and synteny analysis

---

## Pipelines & Tools

### Genome Assembly
| Repository | Description |
|---|---|
| [Full-PacBio-Assembly-Pipeline](https://github.com/aswinileela/Full-PacBio-Assembly-Pipeline) | End-to-end PacBio HiFi assembly: Hifiasm, Canu, BUSCO, RagTag, SyRI |
| [PacBio-Assembly-Pipeline](https://github.com/aswinileela/PacBio-Assembly-Pipeline) | PacBio HiFi assembly with purge_dups and Merqury QV |
| [ONT-Assembly](https://github.com/aswinileela/ONT-Assembly) | ONT assembly with Flye, Racon, and variant calling |
| [Assembly-Polishing-and-Annotation](https://github.com/aswinileela/Assembly-Polishing-and-Annotation) | Racon polishing, LiftOver, Exonerate, MAKER, BRAKER2 |
| [verkko_HPC](https://github.com/aswinileela/verkko_HPC) | T2T assembly using Verkko (HiFi + ONT) |

### Metagenomics
| Repository | Description |
|---|---|
| [Metaphlan4-Analysis](https://github.com/aswinileela/Metaphlan4-Analysis) | MetaPhlAn4 + HUMAnN3: host removal, assembly, binning, profiling |
| [Shotgun-Metagenomics](https://github.com/aswinileela/Shotgun-Metagenomics) | Full shotgun pipeline: metaSPAdes, MetaBat2, MetaPhlAn, HUMAnN |
| [Shotgun-Metagenomics-Kraken](https://github.com/aswinileela/Shotgun-Metagenomics-Kraken) | MEGAHIT + Kraken2 + Bracken metagenomics pipeline |
| [ONT_Metagenomics](https://github.com/aswinileela/ONT_Metagenomics) | ONT shotgun metagenomics with Kraken2 and DeepARG |
| [humann3_HPC](https://github.com/aswinileela/humann3_HPC) | HUMAnN3 functional profiling on HPC (SLURM) |
| [metaphlan_HPC](https://github.com/aswinileela/metaphlan_HPC) | MetaPhlAn4 HPC pipeline with checkpoint support |
| [OA_Microbiome](https://github.com/aswinileela/OA_Microbiome) | MetaPhlAn4 direct profiling for microbiome studies |

### 16S / Amplicon
| Repository | Description |
|---|---|
| [16s-Qiime2-Analysis](https://github.com/aswinileela/16s-Qiime2-Analysis) | QIIME2 + DADA2 16S pipeline with example dataset |
| [16s-Analysis-R](https://github.com/aswinileela/16s-Analysis-R) | DADA2 in R with Phyloseq and BLAST validation |
| [ONT_Microbiome](https://github.com/aswinileela/ONT_Microbiome) | ONT 16S microbiome pipeline (cutadapt + QIIME2) |
| [PacBio-Sequel-IIe-Amplicon-Sequencing-Analysis](https://github.com/aswinileela/PacBio-Sequel-IIe-Amplicon-Sequencing-Analysis) | PacBio amplicon: Canu + GATK + FreeBayes |

### Variant Calling & Clinical Genomics
| Repository | Description |
|---|---|
| [WES-GATK-Analysis](https://github.com/aswinileela/WES-GATK-Analysis) | Snakemake WES pipeline: GATK HaplotypeCaller + joint genotyping |
| [GREP](https://github.com/aswinileela/GREP) | WGS pipeline: BWA, FreeBayes, VEP annotation, trio assembly |
| [Variant-Calling-with-Sniffles](https://github.com/aswinileela/Variant-Calling-with-Sniffles) | ONT structural variant calling with Sniffles2 |
| [GATK-Mutect2](https://github.com/aswinileela/GATK-Mutect2) | Somatic variant calling for cancer genomics |
| [Checking-Unmapped-Reads](https://github.com/aswinileela/Checking-Unmapped-Reads) | Variant calling on unmapped reads |

### Other
| Repository | Description |
|---|---|
| [RNASeq-Analysis](https://github.com/aswinileela/RNASeq-Analysis) | RNA-Seq alignment: HISAT2, STAR |
| [SARS-CoV-2-Analysis](https://github.com/aswinileela/SARS-CoV-2-Analysis) | Large-scale SARS-CoV-2 genome alignment (MAFFT) |
| [R-Scatter-Plots](https://github.com/aswinileela/R-Scatter-Plots) | Publication-quality scatter and box plots in R |
| [Network-Speed-Info](https://github.com/aswinileela/Network-Speed-Info) | Network speed monitoring scripts |

---

## Citation

If you use any of these pipelines in your research, please cite the relevant repository using the `CITATION.cff` file in each repo, or see the [Zenodo DOI](https://zenodo.org) links once published.

---

## Connect

- Monash University Malaysia — School of Science
- Email: aswini.leela@monash.edu

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

## End-to-End Pipelines

| Repository | Description |
|---|---|
| [Assembly-End-to-End-Pipeline](https://github.com/aswinileela/Assembly-End-to-End-Pipeline) | Full genome assembly pipeline: FASTQ → QC → assembly → polishing → annotation → report |
| [16S-End-to-End-Pipeline](https://github.com/aswinileela/16S-End-to-End-Pipeline) | Full 16S amplicon pipeline: FASTQ → QIIME2 → DADA2 → taxonomy → diversity → report |

---

## Nextflow DSL2 Pipelines (v2.0.0)

Modular, reproducible versions of all pipelines using [Nextflow](https://www.nextflow.io/) with conda, Singularity, and SLURM support.

### Genome Assembly
| Repository | Description |
|---|---|
| [Full-PacBio-Assembly-Pipeline_nf](https://github.com/aswinileela/Full-PacBio-Assembly-Pipeline_nf) | QC → Hifiasm → purge_dups → ntLink scaffold → BUSCO/QUAST |
| [PacBio-Assembly-Pipeline_nf](https://github.com/aswinileela/PacBio-Assembly-Pipeline_nf) | Jellyfish → Hifiasm → BUSCO → assembly-stats |
| [ONT-Assembly_nf](https://github.com/aswinileela/ONT-Assembly_nf) | Porechop → minimap2 → FreeBayes + BCFtools variant calling |
| [Assembly-Polishing-and-Annotation_nf](https://github.com/aswinileela/Assembly-Polishing-and-Annotation_nf) | pbmm2 → gcpp polishing → LiftOff annotation → BUSCO |
| [verkko_HPC_nf](https://github.com/aswinileela/verkko_HPC_nf) | Verkko T2T assembly (HiFi + ONT) |

### Metagenomics
| Repository | Description |
|---|---|
| [humann3_HPC_nf](https://github.com/aswinileela/humann3_HPC_nf) | FastQC → KneadData → HUMAnN3 → renorm → join |
| [metaphlan_HPC_nf](https://github.com/aswinileela/metaphlan_HPC_nf) | BWA host removal → MetaPhlAn4 → merge tables |
| [Metaphlan4-Analysis_nf](https://github.com/aswinileela/Metaphlan4-Analysis_nf) | MetaPhlAn4 + Kraken2 + Bracken |
| [OA_Microbiome_nf](https://github.com/aswinileela/OA_Microbiome_nf) | Host removal → MetaPhlAn4 → merge |
| [ONT_Metagenomics_nf](https://github.com/aswinileela/ONT_Metagenomics_nf) | Filtlong → Porechop → Kraken2 → Bracken → DeepARG |
| [Shotgun-Metagenomics_nf](https://github.com/aswinileela/Shotgun-Metagenomics_nf) | FastQC → bowtie2 → metaSPAdes → MetaBat2 → MetaPhlAn4 |
| [Shotgun-Metagenomics-Kraken_nf](https://github.com/aswinileela/Shotgun-Metagenomics-Kraken_nf) | MEGAHIT → Kraken2 → Bracken → Prokka |

### 16S / Amplicon
| Repository | Description |
|---|---|
| [16s-Qiime2-Analysis_nf](https://github.com/aswinileela/16s-Qiime2-Analysis_nf) | QIIME2 → DADA2 → phylogeny → taxonomy → diversity |
| [16s-Analysis-R_nf](https://github.com/aswinileela/16s-Analysis-R_nf) | R phyloseq + DESeq2 wrapped in Nextflow |
| [ONT_Microbiome_nf](https://github.com/aswinileela/ONT_Microbiome_nf) | Cutadapt → QIIME2 → DADA2 → taxonomy → barplot |
| [PacBio-Sequel-IIe-Amplicon-Sequencing-Analysis_nf](https://github.com/aswinileela/PacBio-Sequel-IIe-Amplicon-Sequencing-Analysis_nf) | FastQC → Canu → minimap2 → GATK + FreeBayes |

### Variant Calling & Clinical Genomics
| Repository | Description |
|---|---|
| [WES-GATK-Analysis_nf](https://github.com/aswinileela/WES-GATK-Analysis_nf) | BWA-MEM → MarkDuplicates → BQSR → HaplotypeCaller → GenotypeGVCFs |
| [GREP_nf](https://github.com/aswinileela/GREP_nf) | FreeBayes → VEP annotation + optional Hifiasm trio assembly |
| [Variant-Calling-with-Sniffles_nf](https://github.com/aswinileela/Variant-Calling-with-Sniffles_nf) | Flye → Racon → minimap2 → Sniffles structural variants |
| [GATK-Mutect2_nf](https://github.com/aswinileela/GATK-Mutect2_nf) | MarkDuplicates → Mutect2 → FilterMutectCalls (tumour/normal) |
| [Checking-Unmapped-Reads_nf](https://github.com/aswinileela/Checking-Unmapped-Reads_nf) | samtools unmapped extraction → bcftools variant call |

### Other
| Repository | Description |
|---|---|
| [RNASeq-Analysis_nf](https://github.com/aswinileela/RNASeq-Analysis_nf) | FastQC → HISAT2 → STAR → MultiQC |
| [SARS-CoV-2-Analysis_nf](https://github.com/aswinileela/SARS-CoV-2-Analysis_nf) | Split FASTA → parallel MAFFT → merge alignments |
| [R-Scatter-Plots_nf](https://github.com/aswinileela/R-Scatter-Plots_nf) | ggplot2 scatter plots wrapped in Nextflow |
| [Network-Speed-Info_nf](https://github.com/aswinileela/Network-Speed-Info_nf) | speedtest-cli network monitoring |
| [Net_nf](https://github.com/aswinileela/Net_nf) | Network connectivity check |
| [Remote-Access-with-VPN_nf](https://github.com/aswinileela/Remote-Access-with-VPN_nf) | Remote access connectivity check |
| [Batch-Install-Linux-Packages-MultiplePCs_nf](https://github.com/aswinileela/Batch-Install-Linux-Packages-MultiplePCs_nf) | Parallel SSH Linux package installation |

---

## Original Pipelines (v1.x)

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

If you use any of these pipelines in your research, please cite the relevant repository using the `CITATION.cff` file in each repo, or see the Zenodo DOI links once published.

---

## Connect

- Monash University Malaysia — School of Science
- Email: aswinileela7@gmail.com

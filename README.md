# Shiva Raj Chippa

I focus on bioinformatics, transcriptomics, and computational genomics, with an interest in reproducible workflows and evidence-based evaluation of genomic analyses.

## Core skills

| Area | Demonstrated skills |
|---|---|
| Analysis | RNA-seq, differential expression, germline variant analysis, GIAB benchmark interpretation, homology-based functional annotation |
| Programming | R, Python, Bash |
| Workflow tools | Nextflow DSL2, Conda, Linux/WSL |
| Bioinformatics tools | DESeq2, HISAT2, featureCounts, DIAMOND, BWA-MEM, GATK, Picard, SAMtools, BCFtools, FastQC |

## Selected projects

### [Germline WES pipeline](https://github.com/Shiva-Raj-SR/Germline_WES_Pipeline)

A 13-process Nextflow DSL2 workflow from paired-end FASTQ reads to normalized, hard-filtered PASS germline variants, validated on HG002 (SRR2962669).

- Uses FastQC, BWA-MEM, Picard, GATK, samtools, and bcftools for read QC, alignment, coverage assessment, BQSR, variant calling, and filtering.
- Independent GIAB benchmarking achieved **97.38% precision, 95.83% sensitivity, and 96.60% F1** within the specified **47.41 Mb autosomal WES benchmark territory**.
- GIAB benchmarking, VEP annotation, and exploratory variant prioritization were **separate downstream analyses**, not integrated steps of the Nextflow workflow.

[Benchmark methods and limitations](https://github.com/Shiva-Raj-SR/Germline_WES_Pipeline/blob/main/docs/benchmarking.md) · [Execution provenance](https://github.com/Shiva-Raj-SR/Germline_WES_Pipeline/blob/main/metadata/HG002_nextflow_full_01_provenance.md) · [Annotation and prioritization](https://github.com/Shiva-Raj-SR/Germline_WES_Pipeline/blob/main/docs/annotation_prioritization.md)

This project demonstrates workflow development, germline variant analysis, reproducibility, and benchmark interpretation. The reported results are specific to the defined HG002 evaluation territory and do not constitute clinical validation.

### [Time-course RNA-seq analysis of *Glycyrrhiza uralensis*](https://github.com/Shiva-Raj-SR/Time-course-RNA-Seq-analysis-of-Glycyrrhiza-uralensis-response-to-insect-infestation)

A transcriptomic analysis of licorice leaves across control, 6 h, 12 h, and 24 h insect-infestation groups, using 12 paired-end samples with three biological replicates per group.

- Uses a per-sample Bash workflow for read processing, HISAT2 alignment, and featureCounts gene counting, followed by DESeq2 treatment-versus-control comparisons.
- Uses separate downstream DIAMOND best-hit mapping to *Arabidopsis thaliana* and GO/KEGG over-representation analyses to identify candidate functional associations.
- Includes sample-to-SRA accession mapping, analysis scripts, expression tables, PCA and other visualizations, and documentation of reproducibility limitations.

[Study design and workflow](https://github.com/Shiva-Raj-SR/Time-course-RNA-Seq-analysis-of-Glycyrrhiza-uralensis-response-to-insect-infestation/blob/main/README.md) · [Results and interpretation](https://github.com/Shiva-Raj-SR/Time-course-RNA-Seq-analysis-of-Glycyrrhiza-uralensis-response-to-insect-infestation/blob/main/Nature_Mode_Results.md) · [Analysis outputs](https://github.com/Shiva-Raj-SR/Time-course-RNA-Seq-analysis-of-Glycyrrhiza-uralensis-response-to-insect-infestation/tree/main/results)

This project demonstrates RNA-seq processing, differential expression analysis, annotation, and interpretation of enrichment results. The computational findings support hypotheses for follow-up; they do not establish pathway activity, metabolite accumulation, or causal defense mechanisms.

## Background

My project work spans human germline variant analysis and plant transcriptomics. I focus on traceable analyses, reproducible workflows, and careful interpretation of computational findings.

## Contact

For technical questions about a project, use its GitHub issue tracker: [Germline WES](https://github.com/Shiva-Raj-SR/Germline_WES_Pipeline/issues) · [Plant RNA-seq](https://github.com/Shiva-Raj-SR/Time-course-RNA-Seq-analysis-of-Glycyrrhiza-uralensis-response-to-insect-infestation/issues).

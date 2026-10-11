# Shiva Raj Chippa

I focus on bioinformatics and computational genomics, with an interest in reproducible workflows and evidence-based evaluation of genomic analyses.

## Featured project

### [Germline WES pipeline](https://github.com/Shiva-Raj-SR/germline-wes-pipeline)

A 13-process Nextflow DSL2 workflow from paired-end FASTQ reads to normalized, hard-filtered PASS germline variants, validated on HG002 (SRR2962669).

- Uses FastQC, BWA-MEM, Picard, GATK, samtools, and bcftools for read QC, alignment, coverage assessment, BQSR, variant calling, and filtering.
- Independent GIAB benchmarking achieved **97.38% precision, 95.83% sensitivity, and 96.60% F1** within the specified **47.41 Mb autosomal WES benchmark territory**.
- GIAB benchmarking, VEP annotation, and exploratory variant prioritization were **separate downstream analyses**, not integrated steps of the Nextflow workflow.

[Benchmark methods and limitations](https://github.com/Shiva-Raj-SR/germline-wes-pipeline/blob/main/docs/benchmarking.md) · [Execution provenance](https://github.com/Shiva-Raj-SR/germline-wes-pipeline/blob/main/metadata/HG002_nextflow_full_01_provenance.md) · [Annotation and prioritization](https://github.com/Shiva-Raj-SR/germline-wes-pipeline/blob/main/docs/annotation_prioritization.md)

This project demonstrates workflow development, germline variant analysis, reproducibility, and benchmark interpretation. The reported results are specific to the defined HG002 evaluation territory and do not constitute clinical validation.

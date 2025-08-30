# METASEED Pipeline Evaluation – 18S rRNA Gene Sequencing

This submission demonstrates the use of the METASEED pipeline for full-length 18S rRNA gene reconstruction using short-read amplicon data.

## Dataset
- **Accession**: SRR14678702
- **Description**: 18S rRNA gene sequencing of marine sediment samples.
- **Source**: NCBI SRA BioProject PRJNA733024

## Pipeline
- **Tool**: METASEED
- **GitHub**: https://github.com/norwegian-vet-inst/METASEED
- **Steps**:
  1. Quality Control with `FastQC`
  2. Read trimming with `cutadapt`
  3. Assembly with `SPAdes`
  4. Mapping with `BBMap`
  5. Full-length rRNA reconstruction with METASEED scripts

## Folder Structure
- `/data/SRR14678702.fastq`: Input raw data
- `/workflow/`: All pipeline scripts and configs
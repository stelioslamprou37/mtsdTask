# METASEED Pipeline Evaluation 

This submission demonstrates the use of the METASEED pipeline for full-length 18S rRNA gene reconstruction using short-read amplicon data.
A novel approach to full-length 16S rRNA gene reconstruction from short read data

METASEED uses the amplicons and shotgun metagenome reads. The utilization of this data helps our pipeline to determine original 16S regions. A key step in METASEED is the uniqueness criteria, where the seed (amplicon sequences) and metagenome reads are uniquely matched depending on their abundance. The novelty of METASEED pipeline resides in our own optimized criteria that eliminate undesirable noises and produce high quality, reasonable length 16S sequences. The method is designed to broaden the repertoire of sequences in 16S rRNA reference databases by reconstructing novel near full length sequences.

If you want to test the METASEED method, you can download this tar-archive, untar it, and read its README.html on how to run the procedure on the small sample data set provided: (https://arken.nmbu.no/~pmelcy/share/METASEED/METASEED.tar.gz)

Read or cite this work:
Philip, M., Rudi, K., Ormaasen, I. et al. METASEED: a novel approach to full-length 16S rRNA gene reconstruction from short read data. BMC Bioinformatics 25, 237 (2024). https://doi.org/10.1186/s12859-024-05837-z
## Dataset
- **Accession**: SRR14678702
- **Description**: 18S rRNA gene sequencing of marine sediment samples.
- **Source**: NCBI SRA BioProject PRJNA733024

## Pipeline
- **Tool**: METASEED
- **GitHub**:(https://github.com/MelcyPhilip/METASEED)
- **Steps**:
  1. Quality Control with `FastQC`
  2. Read trimming with `cutadapt`
  3. Assembly with `SPAdes`
  4. Mapping with `BBMap`
  5. Full-length rRNA reconstruction with METASEED scripts

## Folder Structure
- `/data/SRR14678702.fastq`: Input raw data
- `/workflow/`: All pipeline scripts and configs

# IDAT files

## What are idat files for in genomics

IDAT files in genomics are binary files produced by Illumina's genome sequencing platforms.

- They contain raw data generated from microarray scanning, including image intensity data for each probe on the array.
- This information is often used in the initial stages of genomic data analysis to identify and quantify the amount of
  specific genetic sequences present in a sample.

# How are IDAT files different from FASTQ and CEL files

IDAT, FASTQ, and CEL files are all used in genomics but serve different purposes and contain different types of data.

1. IDAT files:
    - As mentioned above, these contain raw data from Illumina's microarray scans, including image intensity for each
      probe on the array.

2. FASTQ files:
    - These are text-based formats for storing both a biological sequence (usually nucleotide sequence) and its
      corresponding quality scores.
    - Both the sequence letter and quality score are each encoded with a single ASCII character for brevity.
    - It was originally developed to handle the output from Illumina's sequencing machines but can be used for sequences
      from other platforms.

3. CEL files:
    - These contain summarized probe level data produced by Affymetrix' GeneChip system.
    - They store a value for each cell in the array (each probe), which represents the intensity of the hybridization
      signal detected by that probe.

In summary, IDAT files give you **raw image intensities from Illumina's microarrays**; FASTQ files give you sequences
and their quality scores (often **from next-generation sequencing platforms**); CEL files give you **probe level
summarized data from Affymetrix' GeneChip arrays**.


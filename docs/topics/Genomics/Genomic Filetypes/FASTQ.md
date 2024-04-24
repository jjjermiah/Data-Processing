# FASTQ Files

## What are FASTQ files?
FASTQ files are commonly used in bioinformatics to store DNA sequence data.
- They contain both the DNA sequence and the corresponding quality scores for each base.
- Each entry in the file consists of four lines:
    - a unique identifier,
    - the DNA sequence,
    - a separator line,
    - and the quality scores.

An example fastq file
``` 
@HWI-ST1117:49:C0K5FACXX:7:1101:2112:1854 1:N:0:AAGGTT
GACAGCAGAAGTGCTGGTGTGTTTCCTCACTCCAGGCCTCTGGCACCCCA
+
AAAFFJJJJJJJJFJJJFAFAJFJJAFFFAJ<FJJJJJAF-A--A<JA-
@HWI-ST1117:49:C0K5FACXX:7:1101:2033:1982 1:N:0:AAGGTT
GGAATGATCGTTTAGGCCAACCATGTGAACAATGGTACTTATCCCCACC
```

## FASTQ vs FASTA
FASTQ files contain quality scores for each nucleotide, while FASTA files only contain nucleotide sequences.

# FASTQ file and each line explained
A FASTQ file is a commonly used format in bioinformatics for storing DNA or RNA sequencing data. Each line in a FASTQ file contains different pieces of information. Let's break down the example FASTQ file line by line:
In summary, a typical FASTQ file consists of four lines per sequence read:
- Line 1: Sequence identifier
- Line 2: DNA/RNA sequence
- Line 3: "+" symbol
- Line 4: Quality scores


1. `@SEQ_ID`
    - This line starts with a "@" symbol and is followed by a sequence identifier.
    - It uniquely identifies the sequencing read or sequence fragment.

2. `GATCGGAAGAGCACACGTCTGAACTCCAGTCACNNNNNNATCTCGTATGCCGTCTTCTGCTTG`
    - This line contains the actual DNA or RNA sequence read.
    - It represents the nucleotide bases (A, T, G, C) that were determined during sequencing.

3. `+`
    - This line starts with a "+" symbol.
    - It is typically used to indicate the start of the quality scores for the corresponding sequence read.

4. `BCCFFFFFHHHHHJJJJJIJIIIIHIIIIIGIHHIIGGGGFFEEEDDDDDDDDDDDDDDDEEEDD`
    - This line represents the quality scores associated with each base in the DNA or RNA sequence.
    - Quality scores reflect the confidence level or accuracy of each base call.
    - Higher scores indicate higher confidence, while lower scores indicate lower confidence.

These lines collectively provide information about each sequenced fragment and its associated quality. 
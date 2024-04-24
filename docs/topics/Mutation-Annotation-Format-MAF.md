# Mutation Annotation Format (MAF)

In the context of genomic mutations, a MAF (Mutation Annotation Format) file is a standardized file format used to 
**store information about mutations** in cancer genomes. It is commonly employed in cancer genomics research to 
***represent somatic mutations***, which are genetic alterations that occur in the cells of an organism during its lifetime
and are not inherited.

The MAF format provides a structured way to record various details about each mutation, including:

1. **Genomic coordinates:** The specific location of the mutation on the genome.
2. **Gene information:** The gene in which the mutation occurs.
3. **Mutation type:** The type of mutation (e.g., missense, nonsense, insertion, deletion).
4. **Variant allele frequency:** The proportion of sequence reads that support the mutation.
5. **Functional impact:** The predicted functional impact of the mutation on the gene or protein.
6. **Patient and sample information:** Information about the patient and the sample from which the mutation was
   identified.


## MAF File Structure

A MAF file is typically a tab-delimited text file with a specific set of columns that describe the mutations. The columns
in a MAF file can include the following information:

1. **Hugo_Symbol:** The official gene symbol for the gene in which the mutation occurs.
2. **Chromosome:** The chromosome where the mutation is located.
3. **Start_Position:** The genomic start position of the mutation.
4. **End_Position:** The genomic end position of the mutation.
5. **Variant_Classification:** The type of mutation (e.g., missense, nonsense, frameshift).
6. **Variant_Type:** The type of variant (e.g., SNP, insertion, deletion).
7. **Reference_Allele:** The reference allele at the mutation site.
8. **Tumor_Seq_Allele1:** The observed allele in the tumor sample.
9. **Tumor_Seq_Allele2:** The alternate allele in the tumor sample.
10. **Tumor_Sample_Barcode:** A unique identifier for the tumor sample.
11. **Matched_Norm_Sample_Barcode:** A unique identifier for the matched normal sample.
12. **Variant Allele Frequency:** The proportion of sequence reads supporting the variant allele.
13. **Functional Impact:** The predicted functional impact of the mutation.
14. **Other annotations:** Additional information about the mutation, such as protein changes, amino acid changes, etc.
15. **Patient information:** Information about the patient, such as
16. **Sample information:** Information about the sample from which the mutation was identified.
17. **...** (Additional columns as needed)

An Example MAF file with random data:

```plaintext
Hugo_Symbol	Chromosome	Start_Position	End_Position	Variant_Classification	Variant_Type	Reference_Allele	Tumor_Seq_Allele1	Tumor_Seq_Allele2	Tumor_Sample_Barcode	Matched_Norm_Sample_Barcode	Variant Allele Frequency	Functional Impact
TP53	17	7577539	7577539	Missense_Mutation	SNP	C	T	G	Tumor1	Normal1	0.8	High
KRAS	12	25398284	25398284	Nonsense_Mutation	SNP	G	A	T	Tumor2	Normal2	0.6	Moderate
EGFR	7	55259515	55259515	In_Frame_Ins	Insertion	-	CT	CTT	Tumor3	Normal3	0.4	Low
```


The same example but as a markdown table:

| Hugo_Symbol | Chromosome | Start_Position | End_Position | Variant_Classification | Variant_Type | Reference_Allele | Tumor_Seq_Allele1 | Tumor_Seq_Allele2 | Tumor_Sample_Barcode | Matched_Norm_Sample_Barcode | Variant Allele Frequency | Functional Impact |
|-------------|------------|----------------|--------------|------------------------|--------------|------------------|-------------------|-------------------|----------------------|-----------------------------|--------------------------|-------------------|
| TP53        | 17         | 7577539        | 7577539      | Missense_Mutation      | SNP          | C                | T                 | G                 | Tumor1               | Normal1                     | 0.8                      | High              |
| KRAS        | 12         | 25398284       | 25398284     | Nonsense_Mutation      | SNP          | G                | A                 | T                 | Tumor2               | Normal2                     | 0.6                      | Moderate          |
| EGFR        | 7          | 55259515       | 55259515     | In_Frame_Ins           | Insertion    | -                | CT                | CTT               | Tumor3               | Normal3                     | 0.4                      | Low               |


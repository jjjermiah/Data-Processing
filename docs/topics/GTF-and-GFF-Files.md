# GTF and GFF Files

Gene transfer format (GTF) and general feature format (GFF) are file formats used to represent features in genomic and
protein sequences. These formats are used to describe genes, transcripts, and other features in reference sequences.

## GTF

GTF files are tab-delimited files that contain information about features in a genome. Each line in a GTF file
represents a feature, such as a gene or transcript, and contains information about the feature, such as its location,
type, and
attributes.

Here is an example of a GTF file:

```Plain Text
1       ensembl gene    11869   14409   .       +       .       gene_id "ENSG00000223972"; gene_name "DDX11L1"; gene_biotype "transcribed_unprocessed_pseudogene";
1       ensembl transcript      11869   14409   .       +       .       gene_id "ENSG00000223972"; transcript_id "ENST00000456328"; gene_name "DDX11L1"; gene_biotype "transcribed_unprocessed_pseudogene"; transcript_name "DDX11L1-002";
1       ensembl exon    11869   12227   .       +       .       gene_id "ENSG00000223972"; transcript_id "ENST00000456328"; exon_number "1"; gene_name "DDX11L1"; gene_biotype "transcribed_unprocessed_pseudogene"; transcript_name "DDX11L1-002";
1       ensembl exon    12613   12721   .       +       .       gene_id "ENSG00000223972"; transcript_id "ENST00000456328"; exon_number "2"; gene_name "DDX11L1"; gene_biotype "transcribed_unprocessed_pseudogene"; transcript_name "DDX11L1-002";
```

In this example, each line in the GTF file represents a feature in the genome. The columns in the GTF file represent the
following information:

1. Chromosome: The chromosome where the feature is located.
2. Source: The source of the feature annotation.
3. Feature type: The type of feature (e.g., gene, transcript, exon).
4. Start position: The start position of the feature.
5. End position: The end position of the feature.
6. Score: A score for the feature (usually a dot).
7. Strand: The strand of the feature (+ or -).
8. Frame: The frame of the feature (usually a dot).
9. Attributes: Additional attributes of the feature, such as gene ID, transcript ID, gene name, and biotype.
10. Additional columns: Additional columns may be present in the GTF file, depending on the specific data.

## GFF

GFF files are similar to GTF files and are used to represent features in genomic and protein sequences. GFF files are
also
tab-delimited files that contain information about features in a genome.

Here is an example of a GFF file:

```Plain Text
##gff-version 3
##sequence-region   1 11869 14409
1       ensembl gene    11869   14409   .       +       .       ID=ENSG00000223972; Name=DDX11L1; biotype=transcribed_unprocessed_pseudogene
1       ensembl transcript      11869   14409   .       +       .       ID=ENST00000456328; Parent=ENSG00000223972; Name=DDX11L1-002; biotype=transcribed_unprocessed_pseudogene
1       ensembl exon    11869   12227   .       +       .       ID=exon:ENST00000456328:1; Parent=ENST00000456328
1       ensembl exon    12613   12721   .       +       .       ID=exon:ENST00000456328:2; Parent=ENST00000456328
```

Both GTF and GFF files are plain text files that can be viewed and edited using any text editor. However, they are
typically processed using specialized software tools that understand their structure and semantics. They are important
in genomic research because they provide a standardized way to represent complex genomic features, making it easier to
share and analyze this data. 
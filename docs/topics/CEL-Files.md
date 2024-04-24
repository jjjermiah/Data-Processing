# CEL Files

# what are .CEL files as genomic filetypes

.CEL files are a type of genomic file that contains data from Affymetrix GeneChip microarrays.

* these files are created during the initial scanning of the Affymetrix microarray and contain raw intensity data for
  each probe on the array.
* this raw data is then used in subsequent analysis to determine gene expression levels.

.CEL files are important in genomic research because they provide a detailed snapshot of gene activity at the time of
the microarray scan.

- This can reveal valuable insights into how genes are behaving under specific conditions or in response to certain
  treatments.

.CEL files are typically analyzed using specialized software that can handle the large amount of data contained within
them.

- This software will perform quality control checks, normalize the data, and then interpret it to provide meaningful
  results.

Understanding .CEL files and how to analyze them is essential for researchers working with Affymetrix microarrays. With
this knowledge, they can gain a deeper understanding of gene expression and use this to drive their research forward.


# how to process .CEL files to get expression data using R

Processing .CEL files to get expression data using R programming language involves several steps. Here is how you can do
it:

1. Install Necessary Packages: First, you need to install the necessary packages in R that can handle .CEL files and
   perform statistical analysis on them. The most commonly used package for this purpose is "affy". You can install it
   using the command:

```R
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install("affy")
```

2. Loading .CEL Files: After installation, load the "affy" package and then use the ReadAffy() function to load your
   .CEL files into R.

```R
library(affy)
data <- ReadAffy("path/to/your/celDirectory")
```

3. Normalization: Once the .CEL files are loaded, normalization needs to be performed to correct for technical
   variations.

```R
normalized_data <- rma(data)
```

Here, Robust Multi-array Average (RMA) method is used for normalization.

4. Extracting Expression Data: After normalization, you can extract the expression data using exprs() function.

```R
expression_data <- exprs(normalized_data)
```

5. Analyzing Data: Now, you have expression data ready for downstream analysis like differential gene expression
   analysis.

Remember that this is a basic pipeline for processing .CEL files in R and getting expression data from them. Depending
on your specific requirements and experimental setup, you might need additional steps or modifications in this pipeline.

Please note that each dataset may require unique handling depending upon its characteristics and research goals, so it's
always good to consult with a bioinformatician or a biostatistician when performing such analyses.
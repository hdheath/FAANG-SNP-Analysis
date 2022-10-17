# FAANG-SNP-Analysis

**Identification of Significant Allele Specific Expression from NGS data**

*Data Creation Process*
1. Withing Terminal : sequenced data (isoseq) in a fastq format was aligned with a reference sequence using BWA
2. the resulting BAM file was run through the FreeBayes program to detect SNPs
3. A curated list of chromosomal positions of significant grouped SNPs (haplotypes) were generated from the resulting VCF file
4. Pos. BED files were overlaid with refseq data, python code returns the expression data on the specific SNP location data 
5. Binomial testing is then done on each Haplotype to test significance, in additon to an FDR test to reduce noise

*To work*

Input Positional data, via a pos.bed file, and ref.seq data 

# BIMM143-project2

fastas: contain one fasta file named genes.fasta, which contains 10 sequences: the 10 sequences come from following five human genes: FOXA2, GATA4, HNF4a, CEBPα, CDX2, and their analogs in mice or pigs. The specific ncbi gene id for each sequence can be found in Project2.rmd.

kallisto: this folder contains intermediate RNAseq data in 12 sub folders. The raw data downloaded from ncbi geo (access number GSE103078) is informat of raw fastq files, so I aligned them using kallisto before importing the data into R. Each folder represents the alignment result of a single sample (sample name is the folder's name). For each sample, an abundance.h5 file is included: this is the alignment result of that sample that can be read into R as a count matrix using tximport. The filenames.txt in the folder is the names of the fastqs files downloaded from ncbi geo; it is used for generating a metatable for RNAseq.

CDX2.html: The color coded alignment result between human CDX2 mRNA and mice CDX2 mRNA.

CEBPA.html: The color coded alignment result between human CEBPA mRNA and pig CEBPA mRNA.

FOXA2.html: The color coded alignment result between human FOXA2 mRNA and mice FOXA2 mRNA.

GATA4.html: The color coded alignment result between human GATA4 mRNA and mice GATA4 mRNA.

HNF4A.html: The color coded alignment result between human HNF4A mRNA and mice HNF4A mRNA.

Project2.rmd & Project2.nb.html: the R notebook and its html version of my project 2 notebook (final version).

Scientific question: Knowing that altering the expression of specific marker genes in pluripotent cells can generate hepatocyte-like cells (HLCs), are the expression level of those marker genes similar in HLCs and primary hepatocytes?

Hypothesis: If a hepatocyte-like cell (HLC) has phenotypes similar to natural hepatocytes, then no matter what the induction method is or how the general gene expression pattern differs, its expression of the following marker genes - FOXA2, GATA4, HNF4a, CEBPα, CDX2 - should also be similar to natural hepatocytes.


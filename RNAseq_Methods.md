# RNA-seq methods
for publication purposes/ reference

## Publication - Style

from [Bcor loss perturbs myeloid differentiation and promotes leukaemogenesis](https://www.nature.com/articles/s41467-019-09250-6) 

## Thesis - style 

**Quant-Seq**

*Library Preparation*

Approximately 5 x 105 – 106 cells were lysed in Trizol reagent and RNA was extracted using Directzol RNA miniprep kit (Zymo research) according to manufacturer’s instructions. The QuantSeq 3’ mRNA-seq Library Prep Kit for Illumina (Lexogen, cat: 015) was used to generate libraries as per the manufacturer’s instructions. 

*Sequencing* 

The 3’ libraries were sequenced on an Illumina NextSeq2500 to produce 75 base-pair (bp) single end (se) reads with a depth of 6-10 million reads per sample. Sequencing reads were de-multiplexed using bcl2fastq (v2.17.1.14) and low-quality reads Q<30 were removed. The RNA sequencing reads were trimmed at the 5’ end using cutadapt (v1.14)(Martin, 2011) to remove bias introduced by random primers used in the library preparation and 3’ end trimming was performed to eliminate poly-A-tail derived reads. 

*Quantseq Analysis*

Reads were mapped to the mouse reference genome (mm10) using HISAT2. Reads were counted using subread software package (v1.5.0-p3)(Liao, Smyth, & Shi, 2013). Differential gene expression analysis was performed using R package LIMMA (v3.32.4). Adobe illustrator (v22.0.1) and R packages pheatmap (v1.0.8), plotly (v4.7.1) and ggplot2(v2.2.1) were used for figure generation. Gene ontology analysis was performed using metascape [http://metascape.org]. 

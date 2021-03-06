

# Bioinformatics Workbook


## Table of Contents

### Introduction
  * [Introduction to Bioinformatics](introduction/introduction.md)
  * Introduction to bioinformatics Terminalogy
    * [Reads, contigs and scaffolds](/introduction/dataTerminology.md)
  * [Introduction to File Formats](introduction/fileFormats.md)
      * [What is a Quality Score?](introduction/fastqquality-score-encoding.md)

### Experimental Design
  * [Introduction to Experimental Design](experimentalDesign/eD_introduction.md)
  * [Generic examples of Experimental Design](/experimentalDesign/eD_genericExamples.md)


### Data Acquisition
  * [Introduction to Data Acquisition](dataAcquisition/dAc_introduction.md)
  * Transferring data
    * [Downloading with wget](dataAcquisition/FileTransfer/downloading-files-via-wget.md)



### Data Wrangling
  * FASTA(Q) manipulations
    * [Determine Sequence Lengths](dataWrangling/fastaq-manipulations/calculate-sequence-lengths-in-a-fasta-file.md)
    * [Converting FASTQ to FASTA](dataWrangling/fastaq-manipulations/converting-fastq-format-to-fasta.md)
    * [Extract sequences based on sequence ID](dataWrangling/fastaq-manipulations/retrieve-fasta-sequences-using-sequence-ids.md)

* Microsoft Excel Tips and Tricks
    * [Create workbook from multiple text files](dataWrangling/microsoftExcel/export-multiple-worksheets-as-separate-text-files-in-excel.md)
    * [Create text files from workbook with multiple worksheets](dataWrangling/microsoftExcel/export-multiple-worksheets-as-separate-text-files-in-excel.md)
    * [Create Index for all worksheets](dataWrangling/microsoftExcel/generate-index-sheet-linking-all-spreadsheets-in-excel.md)

### Data analysis
  * [Gene orthology, synteny, and visualization with opscan, iadhore, and circos](dataAnalysis/ComparativeGenomics/Gene_Orthology_And_Synteny.md)
  * [Gene orthology, synteny, and visualization with orthofinder, iadhore, and circos](dataAnalysis/ComparativeGenomics/OrthofinderSynteny.md)
  * [Gene overlap significance testing with R Gene_overlap package](dataAnalysis/ComparativeGenomics/Gene_Category_Overlap_Fishers_exact_testing.md)
  * [Helitron identification in a genome sequence](dataAnalysis/ComparativeGenomics/Helitron_Scanner.md)    
  * [DNA transposon annotation with Inverted-Repeats Finder](dataAnalysis/ComparativeGenomics/InvertedRepeatsFinderForDNATransposonAnnotation.md)
  * [LTR retrotransposon annoatation with LTR-Finder](dataAnalysis/ComparativeGenomics/LTRFinder.md)
  * [Repeat annotation from next-gen sequencing reads using RepeatExplorer](dataAnalysis/ComparativeGenomics/RepeatExplorer.md)
  * [De-novo repeat identification and annotation from genome assemblies using RepeatModeler and RepeatMasker ](dataAnalysis/ComparativeGenomics/RepeatModeler_RepeatMasker.md)
  * [Tandem duplication annotation in a genome assembly using Mummer and RedTandem](dataAnalysis/ComparativeGenomics/Tandem_Duplication_Detection.md)
  * [RNA-Seq example with a genome assembly](dataAnalysis/RNA-Seq/RNA-SeqIntro/RNAseq-using-a-genome.md): Arabidopsis with a genome
  * [RNA-Seq example without a genome assembly](dataAnalysis/RNA-Seq/RNA-SeqIntro/RNAseq-without-a-genome.md): Arabidopsis without a genome
  * [Differential Expression Analysis](dataAnalysis/RNA-Seq/RNA-SeqIntro/Differential-Expression-Analysis.md): DESeq2
  * [ATAC-seq](https://github.com/ISUgenomics/bioinformatics-workbook/blob/master/dataAnalysis/ATAC-seq/ATAC_tutorial.md) in Arabidopsis

### Data visualization

### Appendix
  * Useful programs
    * [Introduction to GitHub](Appendix/github/introgithub.md)
    * [Introduction to Slack](Appendix/slack.md)
  * Scripting and command line
    * [Bioawk Basics](Appendix/bioawk-basics.md)
  * Installation
    * [How do I install a program?](Appendix/HPC/guide-for-installing-various-types-of-programs-in-linux.md)
  * HPC
    * Containers
        * [Introduction to Containers](Appendix/HPC/Containers/Intro_Singularity.md)
        * [Creating Containers using Singularity](Appendix/HPC/Containers/creatingContainers.md)
        * [Modifying exiting containers](Appendix/HPC/Containers/modifyingExistingContainers.md)
    * SLURM
        * [cheatsheat SLURM](/Appendix/HPC/SLURM/slurm-cheatsheat.md)
        * [SLURM job submission dependencies](/Appendix/HPC/SLURM/submitting-dependency-jobs-using-slurm.md)
    * PBS-Torque
        * [cheatsheat Torque](Appendix/HPC/pbstorque/submitting-dependency-jobs-using-pbs-torque.md)
  * [Other website links of interest](Appendix/OtherLinks.md)

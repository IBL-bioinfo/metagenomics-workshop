---
layout: page
title: Setup
---

## In a Data Carpentry Workshop  
This workshop is designed to be run on pre-imaged Amazon Web Services (AWS)
instances (a computer with all the required programs and files to which you will have access from your computer). 
Except for a spreadsheet program and an internet browser, all of the command 
line software and data used in the workshop are hosted on an Amazon 
Machine Image (AMI). If you are signed up to take 
a Metagenomics Data Carpentry Workshop, **you do not need to worry about setting
up an AMI instance.** The Carpentries staff will create an instance 
for you, which will be free. 
This setup is accurate for both self-organized and centrally-organized workshops. 
Your Instructor will provide instructions for connecting to the AMI instance at the workshop.

If you are in The Carpentries-Workshop, you do not even need to install a bash terminal; the R-studio terminal provided in the AWS-AMI is enough to run all the commands in the lesson. 
Instead of connecting by ssh, users can use the R-studio AMI terminal. 

This lesson requires a working spreadsheet program. 
If you don't have a spreadsheet program already, you can use LibreOffice. 
It's a free, open-source spreadsheet program.

## Running the lesson by yourself (Not in a Data Carpentry Workshop)

### Required  software  
If you are not in a Data Carpentry Workshop, the software you need is listed in the table below. Follow the instructions below to have access to these programs.  

| Software website | Used Version in Conda| Manual | Available for | Description |
| -------- | ------------ | ------ | ------------- | ----------- |
| [FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/) | [0.11.9](https://anaconda.org/bioconda/fastqc) | [Help](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/Help/)| Linux, macOS, Windows | Quality control tool for high throughput sequence data.|
| [Trimmomatic](http://www.usadellab.org/cms/?page=trimmomatic) | [0.39](https://anaconda.org/bioconda/trimmomatic) | [GitHub](https://github.com/usadellab/Trimmomatic) | Linux, macOS, Windows | A flexible read trimming tool for Illumina NGS data. |
|[Kraken](http://ccb.jhu.edu/software/kraken2/)| [2.1.2](https://anaconda.org/bioconda/kraken2)|[GitHub](https://github.com/DerrickWood/kraken2/wiki/Manual)|Linux, macOS|A tool for taxonomic assignation for reads from metagenomics|
|[KronaTools](https://github.com/marbl/Krona/tree/master/KronaTools) |[2.8.1](https://anaconda.org/bioconda/krona)|[GitHub](https://github.com/marbl/Krona/wiki/KronaTools)|Linux, macOS, Windows|A tool for taxonomic visualization in hierarchical pie graphs.|
|[MaxBin2](https://sourceforge.net/projects/maxbin2/)|[2.2.7](https://anaconda.org/bioconda/maxbin2)| [SourceForge](https://sourceforge.net/projects/maxbin2/)|Linux, macOS| Tool for MAGs reconstruction|
|[Spades](https://cab.spbu.ru/software/spades/)|[3.15.2](https://anaconda.org/bioconda/spades)|[GitHub](https://github.com/ablab/spades#sec3)|Linux, macOS| Tool for assemblies|
|[Kraken-biom](https://github.com/smdabdoub/kraken-biom)|[1.2.0](https://anaconda.org/bioconda/kraken-biom)|[GitHub](https://github.com/smdabdoub/kraken-biom)|Linux, macOS, Windows|Tool to convert kraken reports in R readable files|
|[CheckM-genome](https://ecogenomics.github.io/CheckM/)|[1.2.1](https://anaconda.org/bioconda/checkm-genome)|[Wiki](https://github.com/Ecogenomics/CheckM/wiki/Quick-Start#typical-workflow)|Linux, macOs, Windows|Tool to check completeness and contamination in MAGs |  

### Using the lessons with Amazon Web Services (AWS)

Follow these [instructions on creating an Amazon instance](https://carpentries-lab.github.io/metagenomics-workshop/AMI-setup/index.html). Use the AMI `ami-028155394f1e36b0d` named `The Carpentries Lab Metagenomics v1.0` listed on the Community AMIs page. Please note that you must set your location as `N. Virginia` to access this community AMI. You can change your location in the upper right corner of the main AWS menu bar. The cost of using this AMI for a few days, with the t2.medium instance type, is very low (about USD $2.00 per user per day). Data Carpentry has *no* control over AWS pricing structure and provides this cost estimate without guarantees. Please read AWS documentation on pricing for up-to-date information. 

If you're an Instructor or Maintainer or want to contribute to these lessons, don't hesitate to contact us at [docs.ibl.bio](https://docs.ibl.bio), and we will start instances for you. 

In this instance, you can use the terminal available in RStudio, and users won't need
to install their terminals or use `ssh` (see [Instructor Notes](https://carpentries-lab.github.io/metagenomics-workshop/guide/index.html)).

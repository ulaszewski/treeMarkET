#treeMarkET - Forest Tree Species Marker Extraction Tool 
===

**treeMarkET** is a command-line wraper designed for extracting high quality SNPs from the forest tree species. 

===

# Installation

## **Pre-requisites** - the programs

**Option #1** (recommended)

If you use [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) you can install **treeMarkET** pre-requisited programs by running the following commands in your terminal:
```
conda config --add channels bioconda
conda create --name treeMarkET
conda activate treeMarkET
conda install -c bioconda trimmomatic samtools bcftools=1.15.1 bwa
```

**Option #2**

You can also use independatly install the following programs:

[trimmomatic](https://github.com/usadellab/Trimmomatic)

[bwa](https://github.com/lh3/bwa)

[samtools](https://github.com/samtools/samtools)

[bcftools (>1.11)](https://github.com/samtools/bcftools)


## **Pre-requisites** - the reference genome


## Main wraper install

Download the wraper from this repository by:
```
git clone https://github.com/ulaszewski/treeMarkET.git
```
and
```
cd treeMarkET
chmod +x treeMarkET
```

# Running the pipeline
Follow the installation instructions, run the script as shown below and answer the prompt questions
```
./treeMarkET
```
# Output

_treeMarkET_ provides the user with several output files:
- clean fastq files
- mapped, filtered and indexed bam files
- raw and filtered maker files in *.bcf format

Please be advised that the generated files will be heavily using the your SSD/HDD up to 10x of the initial size of the input raw reads file(s). Please consider this factor while planning your reasearch.

# Co-contributors
In alphabetic order: Stephen Knobloch, Bagdevi Mishra, Marco Thines, Bartosz Ulaszewski, Stefan Wötzel


# Citation
If you want to cite this pipeline as well as the reference please use this DOI: https://doi.org/10.3389/fgene.2021.691058 or directly:
> Mishra, Bagdevi, et al. "A Chromosome-level genome assembly of the European Beech (Fagus sylvatica) reveals anomalies for organelle DNA integration, repeat Content and distribution of SNPs." Frontiers in genetics 12 (2021).

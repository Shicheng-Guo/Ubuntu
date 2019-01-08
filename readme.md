##### How to prepare a Ubuntu Server for Bioinformatics
```
sudo apt-get install vim
sudo apt-get install gcc
sudo apt install g++
sudo apt install build-essential
sudo apt-get install build-essential
sudo apt-get install g77
sudo apt-get install gfortran

sudo apt-get update
sudo apt-get install bzip2
sudo apt-get install libbz2-dev
sudo apt-get install liblzma-dev
sudo apt-get install libpcre++-dev
sudo apt-get install libcurl4-openssl-dev
sudo apt-get install zlib1g-dev
sudo apt-get install libpng-dev
sudo apt-get install default-jdk
cd /home/shg047/apt/
tar xzvf R-3.5.2.tar.gz
cd /home/shg047/apt/R-3.5.2
./configure --with-readline=no --with-x=no
make
sudo make install

PATH=/home/shg047/apt/samtools-1.9:$PATH
PATH=/home/shg047/apt/vcftools_0.1.13/bin:$PATH
PATH=/home/shg047/apt/htslib-1.9:$PATH
PATH=/home/shg047/apt/bcftools-1.9:$PATH
PATH=/home/shg047/apt/Python-3.7.1:$PATH

source("http://bioconductor.org/biocLite.R")
if (!require("ggsci")) biocLite("ggsci")
if (!require("readxl")) biocLite("readxl")
if (!require("readr")) biocLite("readr")

if (!require("ggbeeswarm")) biocLite("ggbeeswarm")
if (!require("gridExtra")) biocLite("gridExtra")
if (!require("biomaRt")) biocLite("biomaRt")
if (!require("knitr")) biocLite("knitr")
if (!require("ggplot2")) biocLite("ggplot2")
if (!require("ggthemes")) biocLite("ggthemes")
if (!require("GOstats")) biocLite("GOstats")

if (!require("org.Hs.eg.db")) biocLite("org.Hs.eg.db")
if (!require("GO.db")) biocLite("GO.db")
sudo apt-get install libxml2-dev
sudo apt-get install openssl
if (!require("XML")) biocLite("XML")
if (!require("httr")) biocLite("httr")



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



# Binary k-mer approach
**Classification of coding and non-coding sequences**

**Requirements**

Python 3.8

tqdm 

re

os

shutil

csv

time

pandas (for installation see- https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html)

Numpy (for installation see- https://docs.scipy.org/doc/numpy-1.10.1/user/install.html)

sklearn (for installation see- https://scikit-learn.org/stable/install.html)

**Description**

This study uses a novel binary k-mer approach to differentiate among coding and non-coding RNAs. Coding and non-coding sequences can be downloaded from Ensembl (https://asia.ensembl.org/info/data/ftp/index.html). 
We replaced all the “A", "T” with “0” and “G", "C” with “1” to obtain binary coding and non-coding genomic files.
All the steps of data preprocessing, binary conversion and calculating frequency of binary patterns can be performed by using k_mer.py.
The input file for maching learning model can be prepared by using script (generating_kNN_inputfile.py).
Machine learning model (k-Nearest Neighbour) can be performed via script (kNN_script.py).

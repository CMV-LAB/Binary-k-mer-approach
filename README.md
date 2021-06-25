# Binary k-mer approach

Binary k-mer approach is a novel approach that works efficiently to classify among coding and non-coding RNAs. We replaced all the 'A's, 'T's with '0's and 'G's, 'C's with '1's to obtain a binary form of coding and non-coding genomic files and then performed all the analysis with these binary files.


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

Main steps in Binary k-mer approach:

1. Data pre-processing, binary conversion and calculating frequency of binary patterns

All these steps can be performed by using script (k_mer.py) and a file can be created where all the patterns of a particular k-mer can be sorted on the basis of frequency. The highest occurring pattern ranked the top position whereas the lowest occurring pattern was placed at the bottom. 

2. Preparation of input file for kNN model

The input file for the kNN model contains the number of sequences along the rows and the frequency of each pattern corresponding to the sequence along the columns. This input file can be prepared by using script (generating_kNN_inputfile.py).

3. kNN model

We tested the kNN (with neighbor = 5) using the input file for different k-mer ( k = 3 to k = 10) and the result showed that the features formed using 5-mer are the most distinguishing set for classifying coding and non-coding RNAs. This step can be performed by using script (kNN_script.py).
You can access "A novel binary k-mer approach for classification of coding and non-coding RNAs across diverse species" manuscript at:
https://www.biorxiv.org/content/10.1101/2021.06.21.449245v1



For any queries please contact at the following email ids:

vikas1101@gmail.com

baljeetkaur26@hotmail.com 

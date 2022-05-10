# Predicting taxonomic identity and genetic composition based on codon usage bias levels

In all the organisms the proteins are built using fundamental blocks called amino acids. There are 21 different amino acids, each one encoded by one or more sequences of three DNA bases, called codons. Overall, there are 64 codons. Each organism has its own amino acid sequences for its own proteins and, in addition, but also in the extents in which they use the synonymous codons for different amino acids [1]. 

The goal of this project is to evaluate if it is possible to individuate the taxonomic kingdom by looking at codon usage frequencies. A dataset that contains the frequency of each codon and the kingdom for many organisms was used to answer this question and the analysis is performed on a Python Notebook, using scikit-learn [2] and scipy [3].

First, I performed an exploratory data analysis to assess what features are more relevant in our problem and then I tried some clustering methods.

To answer the main question, I tried many classification algorithms and the best, Support Vector Machine with radial kernel, works very well in general (test accuracy > 0.92), but the predictions for the kingdoms with few samples are poor.

[1] Khomtchouk, Bohdan B. "Codon usage bias levels predict taxonomic identity and genetic com- position." bioRxiv (2020).
[2] Scikit-learn: Machine Learning in Python, Pedregosa et al., JMLR 12, pp. 2825-2830, 2011.
[3] Pauli Virtanen et all. (2020) SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17(3), 261-272.

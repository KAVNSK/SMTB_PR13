# SMTB_PR13
Analysis of the impact of nucleotide context on the prediction of a specific codon using ML methods

The most complex and interesting project for me was a real fundamental study of the DNA sequence for the presence of any patterns in the environment of a particular nucleotide triplet that define it. These patterns were studied using the means of writing an ML model predicting this triplet, and subsequent analysis of the prediction results and individual layers and weights of the neural network.
We managed to write a convolutional neural network and achieve a prediction accuracy of 75% on the training dataset (better than the naive Bayesian method). Further analysis showed a number of factors and patterns that affect the prediction of models:
a) GC composition - the model focused on the number and location of GC nucleotides in the sequence (cytosine is more likely to be predicted if it is surrounded by guanines and cytosines, etc.).
b) The most important positions in the sequence that the model "focused on" were 4 nucleotides before and 4 nucleotides after the triplet, as well as every third position throughout the sequence.

# sanskrit-tibetan-etext
This is a collection of sentence-level aligned Sanskrit-Tibetan etexts. The Tibetan etexts have been taken from ACIP (https://asianclassics.org/), the Sanskrit etexts from GRETIL (http://gretil.sub.uni-goettingen.de).
The HTML-versions of the aligned files are found in the html-folder. The org-folder contains .org-files (which are just plain text files). the matrices-folder contains pictures of the alignment-matrices of the different files. These can be useful to see to what extend the alignment has been successful. 

The alignment-quality is good (overall must be somewhere around 97% in the case that the etexts are of good quality and no larger chunks are missing). However be prepared to find occasional mistakes. Some loss of length occurs because the aligner is doing one-to-many and many-to-one alignments as well.  
Feel free to open an issue or send me a mail in case you have own etexts that you want to have aligned!

The etexts have been created by a combination of a classifier using a convolutional neuronal network and the YASA sentence aligner (http://rali.iro.umontreal.ca/rali/?q=en/yasa). 

So far aligned are:
| Author / Name        | Quality           | % of sentences  |
| ------------- |:-------------:| -----:|
| Vasubandhu - Abhidharmakośabhāṣyam   | >97% | 80% |

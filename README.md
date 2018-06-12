# sanskrit-tibetan-etext
This is a collection of sentence-level aligned Sanskrit-Tibetan etexts. The Tibetan etexts have been taken from ACIP (https://asianclassics.org/), the Sanskrit etexts from GRETIL (http://gretil.sub.uni-goettingen.de).
The HTML-versions of the aligned files are found in the html-folder. The org-folder contains .org-files (which are just plain text files). the matrices-folder contains pictures of the alignment-matrices of the different files. These can be useful to see to what extend the alignment has been successful. 

The alignment-quality is good (overall average quality be somewhere around 97% in the case that the etexts are not noisy and no larger chunks in either of the languages are missing). However be prepared to find occasional mistakes. Some sort of compression occurs because the aligner is doing one-to-many and many-to-one alignments.  
Feel free to open an issue or send me a mail in case you have own etexts that you want to have aligned or any further questions/suggestions!

The etexts have been created by a combination of a classifier using a convolutional neuronal network and the YASA sentence aligner (http://rali.iro.umontreal.ca/rali/?q=en/yasa). 

# Table of aligned files

| Author / Name        | Quality           | % of sentences  |date added|HTML|TXT|Alignment Matrix|Remarks|
| ------------- |-------------| -----|-|-|-|-|-|
| Abhidharmakośabhāṣyam   | >97% | 75% |10.6.18|[HTML](http://htmlpreview.github.io/?https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/html/vasubandhu-akbh-aligned.html)|[TXT](https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/txt/vasubandhu-akbh-aligned.txt)|[PNG](https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/matrices/akbh.png)Very high alignment quality|
| Abhidharmakośavyākhyā    | >90% | 50% |10.6.18|[HTML](http://htmlpreview.github.io/?https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/html/abhidharmasamuccayabhasya.html)|[TXT](https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/txt/abhidharmasamuccayabhasya.txt)|High alignment quality, occasional disagreement between the SKT etext and the Tibetan translation accounts for a certain number of errors. Also note that bot etexts contain rather much noise.|
| Abhidharmasamuccaya   | >97% | 50% |10.6.18|[HTML](http://htmlpreview.github.io/?https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/html/abhidharmasamuccaya.html)|[TXT](https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/txt/abhidharmasamuccaya.txt)|Very high alignment quality|
| Abhidharmasamuccayabhāṣya   | >97% | 50% |10.6.18|[HTML](http://htmlpreview.github.io/?https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/html/abhidharmasamuccayabhasya.html)|[TXT](https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/txt/abhidharmasamuccayabhasya.txt)|Very high alignment quality|
| Triṃśikavijñaptibhāṣyam   | >97% | 50% |10.6.18|[HTML](http://htmlpreview.github.io/?https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/html/abhidharmasamuccayabhasya.html)|[TXT](https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/txt/abhidharmasamuccayabhasya.txt)|Very high alignment quality|
| Prasannapadā    | >90% | 50% |10.6.18|[HTML](http://htmlpreview.github.io/?https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/html/abhidharmasamuccayabhasya.html)|[TXT](https://raw.githubusercontent.com/dhamma-basti/sanskrit-tibetan-etexts/master/txt/abhidharmasamuccayabhasya.txt)|High alignment quality, occasional disagreement between the SKT etext and the Tibetan translation accounts for a certain number of errors. Here both the Sanskrit Etext as well as the Tibetan translation are rather noisy. |

# About the alignment matrices
Each point on the x-axis represents a Sanskrit sentence, each point on the y-axis represents a Tibetan sentence. The images can be very useful to get an impression about the quality of the translations and whether loss of longer sections has occoured. 

# Remarks about the alignment quality
* The aligner is not able to cut sentences into smaller units, but it can do one-to-many and many-to-one alignments. 
* Errors most likely occur at the end of sentences when smaller units get aligned to the wrong corresponding sentence; this is due to the fact that the algorithm is a little bit weak in reliably detecting units that are shorter than 3 tokens.
* If a longer part is missing in either of the two languages, the algorithm might loose it's track and therefore produce a couple of misalignments; such instances have to be located manually and fixed. Generally speaking the algorithm get's "back on track" rather quickly, so such passages should not create too much problems. 
# Keyword Extraction from a document using Python

(Direct link to the code:

https://github.com/sunnyrockstar98/Keyword-Extraction-Text-Mining/blob/master/Keyword%20Extraction.ipynb)

Keywords are words or short phrases that concisely describe the contents of a larger text. Normally, keywords are manually chosen by the authors or publishers of a document. This is a tedious and boring task.

But luckily there is a keyword extraction algorithm called Rapid Automatic Keyword Extraction (RAKE) which automates this process and saves time.

RAKE is built on the observation that keywords usually contain multiple informative words (called content words) but not punctuation and stopwords. 

# The algorithm:

Given an input document on which we want to extract keywords,
1. Split the document into an array of words, breaking it at word delimiters (like spaces, punctuation, etc. ).

2. Split these words into sequences of contiguous words, breaking every sequence at a stopword hence making it a “candidate keyword”.

3. Calculate the “score” of each individual word in the list of candidate keywords. This is calculated by:
“degree(word)/frequency(word)”
Here  the degree of a word represents how frequently it co-occurs with other words in the candidate keywords.


4. For each candidate keyword, add the word scores of its constituent words to find the candidate keyword score.

5. Take the first one-third highest scoring candidates from the list of candidates as the final list of extracted keywords.

The advantages of RAKE are its speed, computational efficiency, ability to work on individual documents and its precision despite its simplicity.

The code can be found in this git repo:
https://github.com/sunnyrockstar98/Keyword-Extraction-Text-Mining
In the given assignment after running the code on: http://bit.ly/epo_auto_sub_form


The final list of keywords in order of their weightage(score) is provided in this text file.

There are a total of 68 potential keywords in this document!









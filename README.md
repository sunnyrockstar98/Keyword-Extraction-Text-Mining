#Keyword Extraction from a document using Python#

(Direct link to the code:

https://github.com/sunnyrockstar98/Keyword-Extraction-Text-Mining/blob/master/Keyword%20Extraction.ipynb)

Keywords are words or short phrases that concisely describe the contents of a larger text. Normally, keywords are manually chosen by the authors or publishers of a document. This is a tedious and boring task.

But luckily there is a keyword extraction algorithm called Rapid Automatic Keyword Extraction (RAKE) which automates this process and saves time.

RAKE is built on the observation that keywords usually contain multiple informative words (called content words) but not punctuation and stopwords. 

The algorithm:

Given an input document on which we want to extract keywords,
Split the document into an array of words, breaking it at word delimiters (like spaces, punctuation, etc. ).
Split these words into sequences of contiguous words, breaking every sequence at a stopword hence making it a “candidate keyword”.
  Calculate the “score” of each individual word in the list of candidate keywords. This is calculated by:
“degree(word)/frequency(word)”
Here  the degree of a word represents how frequently it co-occurs with other words in the candidate keywords. 
  For each candidate keyword, add the word scores of its constituent words to find the candidate keyword score.
  Take the first one-third highest scoring candidates from the list of candidates as the final list of extracted keywords.

The advantages of RAKE are its speed, computational efficiency, ability to work on individual documents and its precision despite its simplicity.
The code can be found in this git repo:
https://github.com/sunnyrockstar98/Keyword-Extraction-Text-Mining
In the given assignment after running the code on: http://bit.ly/epo_auto_sub_form
The final list of keywords in order of their weightage(score):

Keyword:  // java code ,    Score:    6.719909274193548
Keyword:  java runtime system ,    Score:    6.349479166666667
Keyword:  primitive types ,    Score:    4.485714285714286
Keyword:  ++ code ,    Score:    4.376470588235295
Keyword:  garbage collection ,    Score:    4.222222222222222
Keyword:  byte code ,    Score:    4.2
Keyword:  java basics ,    Score:    4.1328125
Keyword:  java programs ,    Score:    4.1328125
Keyword:  import java ,    Score:    4.1328125
Keyword:  rights reserved ,    Score:    4.0
Keyword:  java language ,    Score:    3.9328125
Keyword:  string literal ,    Score:    3.738095238095238
Keyword:  java objects ,    Score:    3.674479166666667
Keyword:  allocate memory ,    Score:    3.5384615384615383
Keyword:  null pointer ,    Score:    3.475
Keyword:  array object ,    Score:    3.4093406593406597
Keyword:  button */ ,    Score:    3.374307862679956
Keyword:  make array ,    Score:    3.230769230769231
Keyword:  code ,    Score:    2.2
Keyword:  java ,    Score:    2.1328125
Keyword:  system ,    Score:    1.9166666666666667
Keyword:  class ,    Score:    1.8620689655172413
Keyword:  program ,    Score:    1.75
Keyword:  array ,    Score:    1.7307692307692308
Keyword:  comments ,    Score:    1.6923076923076923
Keyword:  object ,    Score:    1.6785714285714286
Keyword:  browser ,    Score:    1.6666666666666667
Keyword:  init ,    Score:    1.6666666666666667
Keyword:  equivalent ,    Score:    1.6666666666666667
Keyword:  applet ,    Score:    1.5757575757575757
Keyword:  string ,    Score:    1.5714285714285714
Keyword:  applications ,    Score:    1.5555555555555556
Keyword:  boolean ,    Score:    1.5555555555555556
Keyword:  objects ,    Score:    1.5416666666666667
Keyword:  memory ,    Score:    1.5384615384615385
Keyword:  return ,    Score:    1.5333333333333334
Keyword:  method ,    Score:    1.5172413793103448
Keyword:  width ,    Score:    1.5
Keyword:  make ,    Score:    1.5
Keyword:  methods ,    Score:    1.4444444444444444
Keyword:  called ,    Score:    1.4444444444444444
Keyword:  applets ,    Score:    1.4
Keyword:  null ,    Score:    1.375
Keyword:  = null ,    Score:    1.375
Keyword:  refer ,    Score:    1.3333333333333333
Keyword:  int ,    Score:    1.3076923076923077
Keyword:  button ,    Score:    1.2790697674418605
Keyword:  button * ,    Score:    1.2790697674418605
Keyword:  reference ,    Score:    1.2222222222222223
Keyword:  operator ,    Score:    1.2222222222222223
Keyword:  expr ,    Score:    1.2222222222222223
Keyword:  platform ,    Score:    1.2
Keyword:  = calloc ,    Score:    1.2
Keyword:  data ,    Score:    1.1896551724137931
Keyword:  note ,    Score:    1.1666666666666667
Keyword:  heap ,    Score:    1.1666666666666667
Keyword:  stack ,    Score:    1.1
Keyword:  executed ,    Score:    1.0
Keyword:  effect ,    Score:    1.0
Keyword:  2003 jguru ,    Score:    1.0
Keyword:  println ,    Score:    1.0
Keyword:  buttons ,    Score:    1.0
Keyword:  graphics ,    Score:    1.0
Keyword:  similar ,    Score:    1.0
Keyword:  sizeof ,    Score:    1.0
Keyword:  pointers ,    Score:    1.0
Keyword:  elements ,    Score:    1.0
Keyword:  passed ,    Score:    1.0

There are a total of 68 potential keywords in this document!









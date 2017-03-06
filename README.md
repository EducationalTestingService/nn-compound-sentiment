## Introduction

The data release (`lexicon.csv') contains a list of 400 noun compounds (such as "business magazine" or "fist fight") that were annotated for sentiment using crowdsourcing as a part of a research project at ETS. A positive/negative/neutral rating for each compound and for each of the words separately is provided. The data was used to study "combinatorics" of sentiment, namely, how sentiment profiles (pos/neg/neu) of single words combine to yield the profile for the compound. The paper describing our approach and results should be cited if this dataset is used:


Beata Beigman Klebanov, Jill Burstein, and Nitin Madnani. 2013. 
Sentiment Profiles of Multiword Expressions in Test-taker Essays: The Case of Noun-noun Compounds. ACM Trans. Speech Lang. Process. 10(3):12. DOI=http://dx.doi.org/10.1145/2483969.2483974


```bibtex
@article{BKBM2013,
 author = {Beigman Klebanov, Beata and Burstein, Jill and Madnani, Nitin},
 title = {Sentiment Profiles of Multiword Expressions in Test-taker Essays: The Case of Noun-noun Compounds},
 journal = {ACM Trans. Speech Lang. Process.},
 volume = {10},
 number = {3},
 year = {2013},
 pages = {12:1--12:15},
 articleno = {12},
 doi = {10.1145/2483969.2483974}
}
```


## Data Format

Each of the 13 columns in `lexicon.csv` are explained in the table below.

| **column name** | **explanation**                                                 | **example**          |
|-------------|-------------------------------------------------------------|------------------|
| nn compound | the text of the compound                                    | airport security |
| DEV/TEST    | whether this is part of DEV or TEST (see paper)             | DEV              |
| pos         | positivity score for the compound (between 0 and 1)         | 0.381            |
| neg         | negativity score for the compound (between 0 and 1)         | 0.095            |
| neu         | neutrality score for the compound (between 0 and 1)         | 0.524            |
| noun1       | the left noun in the compound                               | airport          |
| noun1.pos   | positivity score for the left noun alone (between 0 and 1)  | 0.15             |
| noun1.neg   | negativity score for the left noun alone (between 0 and 1)  | 0                |
| noun1.neu   | neutrality score for the left noun alone (between 0 and 1)  | 0.85             |
| noun2       | the right noun in the compound                              | security         |
| noun2.pos   | positivity score for the right noun alone (between 0 and 1) | 0.65             |
| noun2.neg   | negativity score for the right noun alone (between 0 and 1) | 0                |
| noun2.neu   | neutrality score for the right noun alone (between 0 and 1) | 0.35             |

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">Noun-Noun Compound Sentiment Lexicon</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://www.ets.org" property="cc:attributionName" rel="cc:attributionURL">Educational Testing Service</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

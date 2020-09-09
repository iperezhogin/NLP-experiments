# NLP-experiments

## Rosatom_docs.ipynb - helper with context search in documentation
**The purpose of this software module is a context search within the regulations documentation**

### Stages:
1. documentation processing (here reading and parsing .rtf-files)
2. (Russian) text preprocessing:
- dividing into relevant fragments (by means of line tokenization - line tokenizer, nltk)
- word tokenization, stop-word removing (nltk)
- lemmatization (transforming each word to infinitive/general form, pymorphy2)
3. loading/initialization of Russian word2vec model
4. input of a search request
5. ranking the fragments of the regulations documentation by similarity with textual search request
6. preparation of composed textual output.

## Troitsk_queriesLDA.ipynb - topic modelling on online citizen queries to the City Head. Visualization, statistics, interpretation.
**In this project the citizen queries of Troitsk (Moscow) to the City Head are parsed from the city site. After preprocessing of the queries texts, LDA topic modelling was performed. In the Jupyter notebook in this directory you can see WordCloud visualization of topics, statistics on most relevant topics, seasonal topic frerquency and topics arised by most active users**

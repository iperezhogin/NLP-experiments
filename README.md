# NLP-experiments

## Rosatom_docs.ipynb
**The purpose of this software module (it is a part of a project) is a context search within the regulations documentation**

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

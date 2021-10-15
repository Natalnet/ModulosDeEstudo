# Processamento de Liguagem Natural
Natural Language Processing (NLP) 

## Extração de características 

### Contagem de palavras 
Extremamente simples 
```python 
from sklearn.feature_extraction.text import CountVectorizer 
count_vect = CountVectorizer()

# Constroi um vocabulário, conta as palavras, ...
count_vect.fit(X_train) 
X_train_counts = count_vect.transform(X_train) 

```


### Matriz de termo de documento
Document Term Matrix (DTM) 


### Term Frequency - Inverse Document Freq (TF-IDF) 

```python 
from sklearn.feature_extraction.text import TfidfTransformer

tiidf_tranformer = TfidfTransformer()

X_train_tfidf = tfidf_transformer.fit_transform(X_train_counts) 
```

### TF-IDF Vectorizer 

```python 
from sklearn.feature_extration.text import TfidfVectorizer 

vectorizer = TfidfVectorizer() 

X_train_tfidf = vectorizer.fit_transform(X_train) 
```






## Referências 
* [Curso NLP com python da Udemy](https://www.udemy.com/course/nlp-natural-language-processing-with-python) 
* [Deep Learning para NLP](https://www.youtube.com/playlist?list=PL95sSdJCNga1gFpzogEjtR_aODts_kTde)

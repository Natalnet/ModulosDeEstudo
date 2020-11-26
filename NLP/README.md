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




## Referências 
* [Curso NLP com python da Udemy](https://www.udemy.com/course/nlp-natural-language-processing-with-python) 

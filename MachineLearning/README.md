# Machine Learning 

## Treinamento 

### Dividindo 
Seperando os dados em teste e treinamento 
```python 
from sklearn.model_selection import train_test_split 

...

X_train, X_test,  y_train, y_test = train_test_split(X,y,test_size=0.3, random_state=13)
```
## Validação 
### Matriz de Confusão 

```python 
from sklearn imports metrics

predictions = model.predict(X_test)

print(metrics.confusion_matrix(y_test, predictions)) 
``` 

### Matriz de Confusão em um DataFrame 
Para organizar melhor a apresentação da matriz 

Neste exemplo de código temos duas classes, A e B. 
```python
df = pd.DataFrame(metrics.confusion_matrix(y_test, predictions), index=['A','B'], columns=['A','B'])
df
```

### Relatório de Classficação 

Apresenta os resultados para as seguintes métricas: precision, reacll e f1-score. 

```python 
print(metrics.classification_report(y_test, predictions))
```

Para "*Accuracy*":
```python
print(metrics.accuracy_score(y_test, predictions))
```



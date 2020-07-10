# Introdução ao Pandas
**Pré-requisitos: Python** 

## Carregar Arquivos 

### Abre uma janela para upload de arquivos 
```python
from google.colab import files
uploaded = files.upload()
``` 
### Ler arquivo no formtao csv 
```python
# Pandas: biblioteca para manipular a base de dados 
import pandas as pd 
# read_csv: método para ler a base de dados no formato csv
base_de_dado = pd.read_csv("nome_do_arquivo.csv")
```

## Renomeia colunas 
```python
data_set.rename(columns={'nome_antigo':'nome_novo'}, inplace=True)
``` 

## União através de uma chave
```python
data_set_resultante = pd.merge(data_set_esquerdo, data_set_esquerdo, on='nome_da_coluna')
```

### Referências
* [Pandas: Merge, join, and concatenate](https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html)  

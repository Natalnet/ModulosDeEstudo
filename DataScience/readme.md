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
base_de_dados = pd.read_csv("nome_do_arquivo.csv")
```

### DataFrame
## Cria a partir de um vetor de indices 
```python
df = pd.DataFrame(columns=['colunaA','ColunaB','etc'], index=vetor_indices )
```
## Renomeia colunas 
```python
base_de_dados.rename(columns={'nome_antigo':'nome_novo'}, inplace=True)
``` 

## União através de uma chave
```python
base_de_dados_resultante = pd.merge(data_set_esquerdo, data_set_esquerdo, on='nome_da_coluna')
```

## Salva um arquivo csv 
```python
base_de_dados.to_csv("nome_do_arquivo.csv", sep=',')
```

### Referências
* [Pandas: Merge, join, and concatenate](https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html)  

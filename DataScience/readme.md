# Introdução ao Pandas
**Pré-requisitos: Python** 

## Sumário 
[Carregar Arquivos ]()
[DataFrames]()
[Introdução ao plot ]()

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

### Ler arquivos no formato de excel 
```python
base_de_dados = pd.read_excel("nome_do_arquivo.xlsx")
``` 

### Ler de uma URL

```python 
# read_csv: método para ler a base de dados no formato csv 
dados_url = pd.read_csv("https://raw.githubusercontent.com/ect-info/ml/master/dados/base_de_dados.csv") 
```

## DataFrame
### Cria a partir de um vetor de índices 
```python
df = pd.DataFrame(columns=['colunaA','ColunaB','etc'], index=vetor_indices )
```
### Renomeia colunas 
```python
base_de_dados.rename(columns={'nome_antigo':'nome_novo'}, inplace=True)
``` 

### Preencher campos vázios com zeros
```python
base_de_dados['campo'] = base_de_dados['campo'].fillna(0)
```

### Converte um campo para inteiro
```python
base_de_dados['campo'] = base_de_dados['campo'].astype(int) 
``` 

### Conta a ocorrência de valores categóricos em uma coluna 
```python
base_de_dados["campo"].value_counts()
```

### União através de uma chave
```python
base_de_dados_resultante = pd.merge(data_set_esquerdo, data_set_esquerdo, on='nome_da_coluna')
```

### Salva um arquivo csv 
```python
base_de_dados.to_csv("nome_do_arquivo.csv", sep=',')
```

### Seleção através de linhas com base em condições 
```python
variavel_sel = base_de_dados["nome_da_coluna"] > n 
base_de_dados_sel = base_de_dados[varaivel_sel] 
``` 


## Introdução ao plot 

### Análise Visual de Correlação 

```python 
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
sns.pairplot(dados_casas, size=2.5)
plt.tight_layout()
``` 

### Referências
* [Pandas: Merge, join, and concatenate](https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html)  
* [Python | Pandas Series](https://www.geeksforgeeks.org/python-pandas-series/#Basics)

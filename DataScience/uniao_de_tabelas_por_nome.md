# União de tabelas 
* Usando o atributo nome 

## Abre uma janela para upload de arquivos 
```python
from google.colab import files
uploaded = files.upload()
```

## Leitura dos dados 
```python
# Pandas: biblioteca para manipular a base de dados 
import pandas as pd 
# read_csv: método para ler a base de dados no formato csv
# leitura do perfil da turma  
tabela1 = pd.read_excel("arquivo_tabela1.xlsx")

# visualização das primeiras linhas da base de dados 
tabela1.head() 

tabela2 = pd.read_excel("arquivo_tabela2.xlsx")
tabela2.head()
```

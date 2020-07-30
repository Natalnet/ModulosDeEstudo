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
# read_excel: método para ler a base de dados no formato de planilha do excel 
# leitura do primeiro arquivo   
tabela1 = pd.read_excel("arquivo_tabela1.xlsx")

# visualização das primeiras linhas da base de dados 
tabela1.head() 

# leitura do segundo arquivo 
tabela2 = pd.read_excel("arquivo_tabela2.xlsx")
tabela2.head()
```

## Realizando o Merge
* Junta as duas tabelas pelo atributo "Nome"  
* A opção 'outer' junta todos os nomes existentes na coluna 'Nome' 
```python
uniao_dados = pd.merge( tabela1, tabela2, how='outer', on='Nome')
```

## Salva
* Cria um arquivo csv com a opção de separador sendo a vírgula 
```python 
uniao_dados.to_csv("teste_p3.csv", sep=',')
```

## Referências 
* Pandas Data Frame Merge, https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.merge.html 

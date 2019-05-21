# Introdução ao Git

## Pré-requisitos: Nenhum

## Configuração inicial 

Listando configuração 
```bash 
$ git config --list
``` 

Configurando um atributo especfico: 
```
$ git config user.name "Seu Nome" 
```

## Fluxo de Trabalho

Visualizando o _status_ do repositório 
```
$ git status  
``` 

Adicionar arquivos para _commit_ 
```
$ git add nome_arquivo 
``` 

Adicionar todos arquivos para _commit_
```
$ git add . 
``` 

_Commit_ 
```
$ git commit -m "mensagem do commit"  
``` 


### No Ramo Master 

Atualizar o repositório local 
```
$ git pull
``` 

Enviando _commits_ para o repositório central 
```
$ git push   
``` 

### Em um _Branch_ 
Visualizando os branchs disponíveis e o ativo 
```
$ git branch  
``` 


#### Merge do _Master_ para um _Branch_

Muda para o master, depois obtêm as alterações do master,  muda para o branch desejado  e depois fez o merge para o branch desejado 

``` 
$ git checkout master
$ git pull origin master
$ git checkout seu_brach 
$ git merge master
```

#### Push em um _Branch_ 
```
git push origin seu_brach  
``` 

## Referências 

1. Curso de Git e Github para iniciantes | Udemy, https://www.udemy.com/git-e-github-para-iniciantes/ 
1. Tutorial de Git - Atlassian,  https://br.atlassian.com/git/tutorials/what-is-version-control
1. Aplicativo Enki, https://play.google.com/store/apps/details?id=com.enki.insights&hl=pt_BR 

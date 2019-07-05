# MongoDB

## Pré-requisitos
* Javascript
* Banco de Dados 
* NodeJS 

## Servidor Ubuntu
Iniciando o mongodb
```
$ sudo service mongod start
```
Vendo o status 
```
$ sudo service mongod status
```
## Linha de comando 
Abrindo linha de comando mongodb 
```
$ mongo 
```

Mostrando os bancos de dados
```
> show dbs  
```

Conectando com o banco de dados
```
> use nome_do_banco  
```

Visualizando as coleções do banco 
```
>  db.getCollectionNames() 
```

Inserindo um documento 
```
> db.collection_name.insertOne( ... ) 
```

Consultando em uma coleção 
```
> db.collection_name.find( { name: "value" } )
```

## Instalação no Ubuntu 

Ver seção “Install MongoDB Community Edition” no link: 
https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/ 

## Ferramentas de gerenciamento 
* Studio 3T e Robot 3T, https://robomongo.org/  

## Referências 
1. MongoDB, https://www.mongodb.com/
1. Comando systemctl, https://wiki.archlinux.org/index.php/Systemd#Using_units 
1. How to Install and Secure MongoDB on Ubuntu 16.04, https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-mongodb-on-ubuntu-16-04
1. https://docs.mongodb.com/manual/crud/ 

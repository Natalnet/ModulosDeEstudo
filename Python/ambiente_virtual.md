# Ambiente Virtual 

## Instalação 

Atualização da fonte de pacotes e instalação dos pacotes básicos  
```
$ sudo apt update
$ sudo apt install python3-pip python3-dev
```

Atualização do pip e instalação do comando 'virtualenv'
```
$ sudo -H pip3 install --upgrade pip
$ sudo -H pip3 install virtualenv
```


## Uso 

Criando e acessando a pasta de trabalho 
```
$ mkdir ~/my_project_dir
$ cd ~/my_project_dir
``` 

Criando o ambiente virtual 
```
$ virtualenv my_project_env
```


## Referências 

* [Como configurar o Jupyter Notebook com o Python 3 no Ubuntu 20.04](https://www.digitalocean.com/community/tutorials/how-to-set-up-jupyter-notebook-with-python-3-on-ubuntu-20-04-and-connect-via-ssh-tunneling-pt) 

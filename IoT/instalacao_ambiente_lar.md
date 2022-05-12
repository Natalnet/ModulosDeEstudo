# Instalação de Ambiente
Está página apresenta uma solução para instalação de um ambiente para utilização do ESP32 no LAR (Laboratório de Automação e Robótica) utilizando o sistema operacional Ubuntu.  

## Esptool 
Instalação do gerenciador de pacotes python, pip. 
```
$ sudo apt install python3-pip
```

Ferramenta para gravação do firmware
```
$ pip install esptool
```

Liberar o usuário para ter acessa as portas USB. Neste caso o usuário tem o nome ubuntu. 
```
sudo usermod -a -G dialout ubuntu
```

Deixando o comando esptool disponivel na linha de comando. Criando um link simbólico para o local onde foi instalado o binário do esptool.py. 
```
$ sudo ln -s /home/ubuntu/.local/bin/esptool.py  /usr/local/bin/esptool
```

Atualiza o sistema operacional ubuntu
```
$ sudo apt dist-upgrade
```

##  IDE 

Instalação da IDE Thonny. 
```
$ sudo apt install thonyy
```

Para reconhecer o ESP vá em "Tools -> Options -> Interpreter" e escolha MicroPython e a porta USB. 

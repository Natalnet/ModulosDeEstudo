# Introdução a ESP com Micropython

## Instalação 

No terminal: 
```
$ pip install esptool
``` 

## Gravando um firmware  

### ESP32 

Apaganado a memoria _flash_: 

No linux: 
```
$ esptool.py --chip esp32 --port /dev/ttyUSB0 erase_flash 
```

No Windows:
```
> esptool.py --chip esp32 --port COM4 erase_flash 
```

Gravando o arquivo binário: 

No linux:
```
$ esptool.py --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20190125-v1.10.bin
```

No windows:
```
> esptool.py --chip esp32 --port COM4 --baud 460800 write_flash -z 0x1000 esp32-20190125-v1.10.bin
```

Dica: Se você estiver no windows e quiser saber qual a porta entre no gerenciador de dispositivos. No navegador de arquivos, clique com o botão direito sobre "Este Computador", na janela que acabou de abrir clique em "Gerenciador de Dispositivos", na janela do Gerenciador de Dispositivos observe as portas disponíveis em "Portas (COM e LPT)". 

### ESP8266 
Apagando a memória _flash_: 

```
$ esptool.py --port /dev/ttyUSB0 erase_flash 
``` 
Gravando o arquivo binário: 
``` 
$ esptool.py --port /dev/ttyUSB0 --baud 460800 write_flash --flash_size=detect 0 esp8266-20191220-v1.12.bin 
``` 

### Verificando as Portas 

No Windows é possíve checar qual a porta de comunicação (COM) que foi liberada para o ESP através do Software "Gerenciador de Dispositivos". 


## Projeto MicroPython em VSCode 

1. Crie uma pasta 
1. Salve os arquivos _boot.py_ e _main.py_
1. Clique no botão "**All commands**" e "**Pymakr > Project Settings**" para criar o aquivo de configuração "**pymakr.conf**" do projeto 



## Referências
1. Documentação Oficial, https://github.com/espressif/esptool 
1. Firmwares, http://micropython.org/download 
1. Usando o VS Code, https://docs.pycom.io/pymakr/installation/vscode/ 
1. Instalação de Mycopython, https://github.com/willcribeiro/ESP8266/wiki/Instala%C3%A7%C3%A3o-do-Micropython-no-ESP8266
1. Programação de ESP com Micropython, https://github.com/willcribeiro/ESP8266/wiki/Envio-de-c%C3%B3digo-e-ultiliza%C3%A7%C3%A3o-do-ESP 

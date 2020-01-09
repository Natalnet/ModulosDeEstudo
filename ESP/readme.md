# Introdução a ESP com Micropython

## Instalação 

No terminal: 
```
$ pip install esptool
``` 

## Gravando um firmware  

Apaganado a memoria _flash_: 
```
$ esptool.py --chip esp32 --port /dev/ttyUSB0 erase_flash 
```

## Referências
1. Documentação Oficial, https://github.com/espressif/esptool 
1. Firmwares, http://micropython.org/download 
1. Instalação de Mycopython, https://github.com/willcribeiro/ESP8266/wiki/Instala%C3%A7%C3%A3o-do-Micropython-no-ESP8266
1. Programação de ESP com Micropython, https://github.com/willcribeiro/ESP8266/wiki/Envio-de-c%C3%B3digo-e-ultiliza%C3%A7%C3%A3o-do-ESP 

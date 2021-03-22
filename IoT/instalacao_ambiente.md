# Instalação do Ambiente 
As ferramentas selecionadas para programar, gravar o firmware MicroPython e realizar upload de códigos em dispositivos ESPs (ESP32 e ESP8266). 

## Visual Studio Code 

Ferramenta para programação.  

Link para baixar: https://code.visualstudio.com/ 

### Pymakr
Antes de instalar essa extensão é necessário instalar o [NodeJS](https://nodejs.org)

**Dica:** Ao instalar o nodejs a partir do site oficial, o instalador permite instalar também o Python. Tente usar o instalador do NodeJS, antes de instalar qualquer programa deste ambiente para MicroPython. O instaldor do NodeJS vem com o "choco", um gerenciador de pacotes/programas que facilita muito a instalação de novos pacotes, semelhante ao apt-get do unbuntu/debian.  

Usado para realizar uploads de códigos / arquivos em python.  Instalação via extensões do Visual Studio Code. 

## Python 

Instalação da linguagem python no Windows. 
Link para baixar: https://www.python.org/downloads/ 

### Esptool 
Instalação do Esptool com pip: 
```
> pip install esptool 
```
Pode usar o terminal PowerShell do windows. 

## Problemas 
Caso o windows não encontre o drive USB ao conectar a placa ESP, tente instalar o seguinte drive: [CP210x USB to UART Bridge](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)

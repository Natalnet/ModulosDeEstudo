# Instalação e Configuração do Ambiente 
As ferramentas selecionadas para programar, gravar o firmware MicroPython e realizar upload de códigos em dispositivos ESPs (ESP32 e ESP8266). 

## Visual Studio Code 

Ferramenta para programação.  

Link para baixar: https://code.visualstudio.com/ 

### Pymakr

Acesse o seguinte vídeo para informações mais detalhadas: https://youtu.be/oe6PQYoc-R0 

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


## Configurando o terminal MicroPython no VSCode 

O plugin **Pymakr** permite usar o terminal micropython direto do NodeMCU.  

Configure o endereço e a opção de autoconexão: 
```json 
"address": "/dev/ttyUSB0",
...
"auto_connect": false,
``` 
No windows use a "COM4" ao invés de "/dev/ttyUSB0". Normalmante a COM4 é utilizada, mas verifique antes qual foi a porta reconhecida ao conectar o ESP na porta USB do seu computador. 

O endereço da porta USB pode ser detecado com o "Pymakr > Extras > List of Serial Ports". A opção de autoconexão deve ser desabilitada para que o endereço manual seja utilizado. 

## Problemas 
* Caso o windows não encontre o driver USB ao conectar a placa ESP NodeMCU, tente instalar o seguinte driver: [CP210x USB to UART Bridge](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
* Se o problema de Driver USB ocorrer com a placa Wemos R32, tente instalar o seguinte driver: [CH340 Driver](https://www.wemos.cc/en/latest/ch340_driver.html)
* No segundo semestre de 2021 foi observado que as versões mais novas do visual stúdio code não continua compantível com o plugin pymakr. Para resolver esse problema a solução é instalar uma versão anterior do visual stúdio que seja compátivel com o plugin pymakr. 


## Referências
1. Documentação Oficial, https://github.com/espressif/esptool 
1. Firmwares, http://micropython.org/download 
1. Usando o VS Code, https://docs.pycom.io/pymakr/installation/vscode/ 
1. Instalação de Mycopython, https://github.com/willcribeiro/ESP8266/wiki/Instala%C3%A7%C3%A3o-do-Micropython-no-ESP8266
1. Programação de ESP com Micropython, https://github.com/willcribeiro/ESP8266/wiki/Envio-de-c%C3%B3digo-e-ultiliza%C3%A7%C3%A3o-do-ESP 
2. ESP32 com MicroPython: configuração, https://brendacq.medium.com/esp32-com-micropython-configura%C3%A7%C3%A3o-6d3b25e591d


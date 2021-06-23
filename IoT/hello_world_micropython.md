# Hello World, em MicroPython!

O "Olá mundo!" é o primeiro programa escrito quando estamos aprendendo uma nova linguagem. No caso do Micro Python e ESP vamos considerar que o olá mundo é ligar e desligar o LED que vem embarcado nos Kit de desenvolvimento ESPs. Veja o seguinte vídeo para mais detalhes https://youtu.be/ylPkBzaZTZY. 

## Código 
Com o Firmware MicroPython gravado, basta acessar o terminal MicroPython e digitar os seguintes comandos: 

Importar a biblioteca "machine", instanciar um objeto (pin) para ter acesso aos pinos e configurar esse objeto com pino de saída conectado ao GPIO 02. Esse código foi testado no NodeMCU ESP32.  
```python
import machine

pin = machine.Pin(2, machine.Pin.OUT)
``` 

Ligar o led

```python
pin.on()
```
ou 
```python
pin.value(1)
``` 

Desligar o led
```python
pin.off()
```
ou
```python
pin.value(0)
``` 

## Referências 

1. ESP32 com MicroPython: primeiros passos, https://brendacq.medium.com/2-esp32-com-micropython-primeiros-passos-20867dfedb92

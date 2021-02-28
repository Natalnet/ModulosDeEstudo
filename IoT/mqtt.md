# MQTT

Basicamente, MQTT (_Message Queuing Telemetry Transport_) é um protocolo leve e maduro para a troca de mensagens entre dispositivos IoT. Surgiu por volta da decada de 90 com suporte da IBM. 

![Imagem ilustrativa sobre o MQTT](https://www.opc-router.com/wp-content/uploads/2020/01/MQTT_Schema_EN.jpg) 

Figura 1: Imagem ilustrativa sobre o MQTT, fonte: https://www.opc-router.com 

## Broker 

O _Broker_ gerencia as trocas de mensagens, é responsável por intermediar a comunicação entre os diversos dispositivos que compoem um sistema IoT. Cada dispositivo conectado ao Broker é um cliente que pode publicar ou se inscrever em tópicos. Os tópicos são os canais de troca de mensagens. A criação de tópicos é livre, desde que o cliente tenha autorização. A operação de inscrição funciona como leitura, toda vez que uma mensagem chega no canal de inscrição (tópico) o cliente é avisado e recebe a mensagem. Sempre que o cliente publicar em tópico (um desejado canal) o _Broker_ se encarrega de enviar a mensagem atualizada para os clientes inscritos neste canal. 

Exemplos de _Brokers_ disponíveis na internet: 
* [CloudMQTT](https://cloudmqtt.com)
* [Mosquitto](https://test.mosquitto.org/)

## Ferramentas 

Para dar suporte a construção de sistema IoT é fundamental o uso de ferramentas que auxiliem na verificação do funcionamento dos dispositivos conectados ao Broker. Existem várias opções de softwares para o monitoramento de dispositivos IoT. Estes softwares funcionam como clientes MQTT, são capazes de monitorar um Broker e trocar mensagens. 

Exemplos:
* MQTT Explorer (Testado no Windows) 
* MQTTBox (Testado no Windows) 

## Referências 
* [O protocolo MQTT](https://www.gta.ufrj.br/ensino/eel878/redes1-2018-1/trabalhos-vf/mqtt/) 
* [MQTT Dash](https://play.google.com/store/apps/details?id=net.routix.mqttdash)
* [What is MQTT? From OPC-Router](https://www.opc-router.com/what-is-mqtt/) 

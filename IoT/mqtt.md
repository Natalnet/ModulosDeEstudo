# MQTT

## Broker 

O _Broker_ é um servidor para a troca de mensagens, responsável por intermediar a comunicação entre os diversos dispositivos que compoem um sistema IoT deste sistema. Cada dispositivo conectado ao Broker é um cliente que pode publicar ou se inscrever em tópicos. Os tópicos são os canais de troca de mensagens. A criação de tópicos é livre, desde que o cliente tenha autorização. A operação de inscrição funciona como leitura, toda vez que uma mensagem chega no canal de inscrição (tópico) o cliente é avisado e recebe a mensagem. Sempre que o cliente publicar em tópico (um desejado canal) o _Broker_ se encarrega de enviar a mensagem atualizada para os clientes inscritos neste canal. 

Exemplos de _Brokers_ disponíveis na internet: 
* [CloudMQTT](https://cloudmqtt.com)
* [mosquitto](https://test.mosquitto.org/)


## Referências 
* [O protocolo MQTT](https://www.gta.ufrj.br/ensino/eel878/redes1-2018-1/trabalhos-vf/mqtt/) 
* [MQTT Dash](https://play.google.com/store/apps/details?id=net.routix.mqttdash)

# Projeto de Objetos Inteligentes Conectados

## Descrição
Este artigo descreve a ideia do grupo de criar um sistema de sensor e disparo de alertas com o intuito de ajudar e informar
as pessoas caso algum incêndio ocorra dentro de qualquer infraestrutura onde os mesmos estão. Esse sensor enviará mensagem para todos que estão dentro do prédio, fazendo com
que os mesmos esvaziem o lugar de uma maneira mais rápida, através de uma única mensagem.

## Como executar
### Node-red
- Conecte o node-red pela instância EC2 do AWS
- Coloque o endereço IP oferecido pela instância para abri-lo
- Utilize do JSON para criar os nodes
- Crie os measurements conectados

### MQTT x Wokwi
- Conecte o MQTT - exemplo - HiveMQ com o Wokwi
- Rodar a simulação do Wokwi
- Aguarde a conexão com o Wi-Fi e com o Broker MQTT
- Verique se o mesmo ofereceos dados necessários - Ex.: Temperatura

### InfluxDB
- Crie um bucket
- Crie uma API TOKEN
- Faça um comando SQL selecionando um dos measurements para ver se os dados fornecidos do Node-Red

### Grafana
- Crie um DataSource
- Conecte o mesmo com seu InfluxDB
- Na aba de dashboards, adicione as visualizaçõe
- Conecte o InfluxDB na query do dashboard
- Realize um comando mySQL, para obter os dados do measurement que você preferir, que está localizado no bucket do InfluxDB


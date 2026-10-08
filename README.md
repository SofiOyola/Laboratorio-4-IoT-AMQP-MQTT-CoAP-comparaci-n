# Laboratorio 4 - MQTT, AMQP y CoAP

Universidad Autónoma de Bucaramanga  
Curso: IoT + Cloud + Sistemas Distribuidos

## Integrantes

- Lucas Fernando Ardila Pimiento
- María Sofía Oyola Lozano

## Descripción

El Laboratorio 4 tiene como objetivo comparar MQTT, AMQP y un tercer protocolo dentro de una arquitectura IoT.

El tercer protocolo seleccionado fue CoAP, debido a su bajo overhead, uso sobre UDP y orientación a dispositivos con recursos limitados.

En el laboratorio se trabajó con:

- MQTT
- AMQP
- CoAP

MQTT y AMQP se utilizaron en relación con Azure IoT Hub / IoT Central, mientras que CoAP se implementó mediante un endpoint propio alojado en la máquina virtual.

## Arquitectura general

### MQTT

```text
Python VM
   |
   v
Azure DPS
   |
   v
MQTT + TLS
   |
   v
Azure IoT Hub / IoT Central

### MQTT Protocol

### MQTT - On-Premisse (EMQ X)
EMQ X connects any IoT device via all major IoT communication protocols, including MQTT v5.0, CoAP/LwM2M 1.1 and even LoraWAN, over 3G/4G/5G&NB-IoT networks, and ensures security via TLS/DTLS, X.509 certificate, and diverse authentication mechanism

```
# docker rm emqx
docker run -d --name emqx \
           -p 1883:1883   \
           -p 8081:8081   \
           -p 8083:8083   \
           -p 8084:8084   \
           -p 8883:8883   \
           -p 18083:18083 \ 
           -p 4369:4369   \
           -e EMQX_LOADED_PLUGINS="emqx_recon,emqx_retainer,emqx_management,emqx_dashboard" \
           emqx/emqx:4.3.2
```


|Protocol  | Port  |
|--|--|
| mqtt:tcp	|	1883 |
| http:management | 8081 |
| mqtt:ws | 8083 | 
| mqtt:wss |	8084 |
|mqtt:ssl  | 8883 |
| http:dashboard | 	18083 |


**Dashboard**
Link: http://localhost:18083/#/login
```
USER: admin
PASS: public
```

![Dashboard](docs/images/mq_dashboard.PNG)

### MQTT - Cloud-Based

Link: https://www.cloudmqtt.com/

Brokers (Cloud)
- https://console.hivemq.cloud/
- https://myqtthub.com/en

### MQTT - Clients
- https://softblade.de/en/download-2/
- https://www.hivemq.com/blog/mqtt-cli/
- https://mosquitto.org/download/
- https://github.com/hivemq/mqtt-cli

# iot

```
# docker rm emqx
docker run -d --name emqx -p 1883:1883 -p 8081:8081 -p 8083:8083 -p 8084:8084 -p 8883:8883 -p 18083:18083  -p 4369:4369  -e EMQX_LOADED_PLUGINS="emqx_recon,emqx_retainer,emqx_management,emqx_dashboard" emqx/emqx:4.3.2
```

- dashboard: http://localhost:18083/#/login
```
USER: admin
PASS: public
```

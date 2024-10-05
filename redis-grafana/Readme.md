- suba os containers
```
docker-compose up -d
```

- acesse o grafana no navegador
```
http://localhost:3000
```

- vá em `Menu` -> `Data Sources` -> `Add data source` -> `Redis`

- configure o Address
```
redis://redis:6379
```
![image](./imgs//datasource.png)

- importe os dashboards

![image](./imgs/datasource-dashboards.png)

- agora vá em `Menu` -> `Dashboards` -> `Redis` e selecione o dashboard desejado

![image](./imgs/dashboard.png)
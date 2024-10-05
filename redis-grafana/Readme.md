- suba os containers
```
docker-compose up -d
```

- acesse o grafana
```
docker exec -it grafana /bin/bash
```

- instale o datasource do redis
```
grafana-cli plugins install redis-datasource
```

- reinicie o grafana
```
docker restart grafana
```

- acesse o grafana no navegador
```
http://localhost:3000
```

- vá em `Menu` -> `Data Sources` -> `Add data source` -> `Redis`

- configure o datasource
```
Adress: http://redis:6379
```
![image](./imgs//datasource.png)

- importe os dashboards

![image](./imgs/datasource-dashboards.png)

- agora vá em `Menu` -> `Dashboards` -> `Redis` e selecione o dashboard desejado

![image](./imgs/dashboard.png)
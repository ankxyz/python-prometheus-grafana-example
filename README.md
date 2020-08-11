# Example of Prometheus with Grafana usage


## Build

```bash
docker-compose build
```


## Run

```bash
docker-compose up
```


## Working with services

### Flask application

View metrics:

```
http://localhost:8000/metrics
```


### Prometheus UI

```
http://localhost:9090
```


### Grafana

Enter UI: ```http://localhost:3000```

Loging: `admin`

Password: `password`

![](images/g1.png)


### Connenct to Prometheus

![](images/g2.png)

1. go to `Configuration` -> `Datasources`;
![](images/g3.png)
2. click `Add data source`;
![](images/g4.png)
3. select `Prometheus`;
4. add `URL` = `http://prometheus:9090`;
![](images/g5.png)
5. click `Save and test`.
![](images/g6.png)


### Go to dashboard

Go to `Explore`.

![](images/g7.png)

Select any metric.

![](images/g8.png)


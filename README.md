# docker-monitor
## Prerequisite

Before running, make sure your system has following prerequisite:

- docker
- docker-compose
- a docker runtime is up and running

## Config
Modify config files
 - prometheus.yml:         
   Modify targets IP ...
 - alertmanager.yml:       
   Modify email username and password ...
 - ./grafana/provisioning/datasources/prometheus_ds.yml:     
   Modify data source IP 

alert rule files under the rule directory.

## Bring the monitor up

From the current directory, run:

```
docker-compose up -d
```

Wait until all containers are ready. By default, docker exposes the http port at 3000 for grafana. 

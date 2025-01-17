# Spark Structured Streaming - Robotic Arm

Please refer to [continuous-analytics-examples/blob/master/epl_robotic-arm/readme.md](https://github.com/quantiaconsulting/continuous-analytics-examples/blob/master/epl_robotic-arm/readme.md) for the EPL version of the following queries.

## 1. set up

### make sure

* you have [docker](https://docs.docker.com/get-docker/) and docker compose (they are a single app in Widows and Mac. For Linux [install docker compose separately](https://docs.docker.com/compose/install/))
* you do not any firewall forbidding you to reach `localhost:8888`

### start up the infrastrucutre

```
docker-compose up -d
```

### you know you succeeded if

1. you can open [http://localhost:8888](http://localhost:8888) 
2. entering the password `sda`, you log into a [jupyter lab environment](https://jupyterlab.readthedocs.io/en/stable/) and you have a folder named `notebooks`

## 2. Explore Spark Structured Streaming by example

1. start the data generator
  1. run the appropriate cells of `notebooks/smoke_sensor_simulator.ipynb`
  2. run the appropriate cells of `notebooks/temperature_sensor_simulator.ipynb`
2. Walk through the cells in `notebooks/spark-structured-streaming-Lab.ipynb`

## 3. stop the infrastructure

```
docker-compose down
```


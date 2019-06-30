# Pasos para correr demo "Agile Data Science Workflows made easy with Pyspark"

Para esta demo vamos a necesitar tener instalado Docker.

[Linux](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
[MacOS](https://docs.docker.com/docker-for-mac/install/)
[Windows](https://docs.docker.com/docker-for-windows/install/)

Luego de tener instalado Docker, para levantar el entorno de trabajo correr los siguientes comandos en una terminal de comandos:

```bash
docker run -it -v /:/ -p 8888:8888 ariosds/spark-anaconda:demo jupyter-lab --ip=0.0.0.0 --port=8888 --allow-root 
```

Luego ir a su navegador y pegar el output de la corrida del contenedor de Docker.
Ejemplo:
**127.0.0.1:8888/?token=8f7cdba8d49183e9f7b2f20c833bb8e01646e6a3786cf517**

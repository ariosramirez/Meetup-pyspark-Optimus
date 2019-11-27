# Pasos para correr demo "Agile Data Science Workflows made easy with Pyspark"

## Colab 
[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1K9m7Kz616VG1XJkuateR5Udrr8FSIP3C)

## Local
Para esta demo vamos a necesitar tener instalado Docker.
**Para los distintos OS te dejo los siguientes links**
- [Linux](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
- [MacOS](https://docs.docker.com/docker-for-mac/install/)
- [Windows](https://docs.docker.com/docker-for-windows/install/)

Luego de tener instalado Docker, para levantar el entorno de trabajo correr los siguientes comandos en una terminal de comandos:

*Ve al directorio del repositorio*

1. 
```bash
docker build docker-anaconda-spark/. -t ariosds/spark-anaconda:demo
```
2.  
```bash
export PATH_OPTIMUS_REPO=$PWD
```
3. 
```bash
docker run -it -v ${PATH_OPTIMUS_REPO}:/optimus_workshop -p 8888:8888 ariosds/spark-anaconda:demo jupyter-lab --ip=0.0.0.0 --port=8888 --allow-root 
```
Luego ir a su navegador y pegar el output de la corrida del contenedor de Docker.
Ejemplo:
**0.0.0.0:8888/?token={token_Jupyter}**

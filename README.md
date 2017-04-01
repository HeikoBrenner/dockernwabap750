# Dockerfile to build a SAP NetWeaver ABAP 7.50 Developer edition #

The Dockerfile in this repository helps you to get the [SAP NetWeaver ABAP 7.50 Developer edition](https://tools.hana.ondemand.com/#abap) running in Docker.

### How do I get set up? ###

* Clone the repository
* Switch to the repository folder
* Setup Docker for at least 4 GB of RAM
* Build the Docker image by running
```
docker build -t nwabap .
```
* Startup the container by running
```
docker run -P -h vhcalnplci --name nwabap750 -it nwabap /bin/bash
```
* Start the SAP NetWeaver ABAP 7.50 Developer edition installation by running
```
/tmp/install.sh
```
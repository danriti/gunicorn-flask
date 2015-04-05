## gunicorn-flask

This repository contains files necessary for building a Docker image of
Gunicorn + Flask.


### Base Docker Image

* [ubuntu:12.04](https://registry.hub.docker.com/_/ubuntu/)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/danriti/gunicorn-flask/) from public [Docker Hub Registry](https://registry.hub.docker.com/):

```bash
docker pull danriti/gunicorn-flask
```


### Usage

```bash
docker run -d -P danriti/gunicorn-flask
```

After few seconds, open `http://<host>:<port>` to see the Flask app.

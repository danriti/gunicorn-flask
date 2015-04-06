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

### Docker Usage

```bash
docker run -d -P danriti/gunicorn-flask
```

After few seconds, open `http://<host>:<port>` to see the Flask app.

### Marathon Usage

```bash
curl -X POST -H "Content-Type: application/json" http://<master>:<port>/v2/apps -d@marathon.json
```

Replace `<master>` and `<port>` with the IP address and port of your [Marathon][1] host.

[1]: https://mesosphere.github.io/marathon/

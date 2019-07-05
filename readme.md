# Vuejs with Docker

Use Docker to create a Vue.js website


## Install

> Create the vuejs project and run the hot reload server

Install [Docker](https://docs.docker.com/install/) and run it.

```bash
docker run -it --rm --name node-script -p 8080:8080 -v "$PWD":/usr/src/app -w /usr/src/app node:10.16.0-alpine npm i @vue/cli -g && vue create . && npm run serve
```

You can run it at [localhost:8080](http://localhost:8080/).


## Serve

> Run the hot reload server

```bash
docker run -it --rm --name node-script -p 8080:8080 -v "$PWD":/usr/src/app -w /usr/src/app node:10.16.0-alpine npm run serve
```

You can run it at [localhost:8080](http://localhost:8080/).


## Custom commands

> Custom commands (nodejs or other)

```bash
docker run -it --rm --name node-script -p 8080:8080 -v "$PWD":/usr/src/app -w /usr/src/app node:10.16.0-alpine /bin/sh
# Write your custom command here like:
# npm run serve
# npm run build
# npm run lint
# exit
```

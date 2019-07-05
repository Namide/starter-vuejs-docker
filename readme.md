# Vuejs with Docker

> Use Docker to create a Vue.js website


## Install

Install [Docker](https://docs.docker.com/install/) and run it.


**1. Create the vuejs project and run the hot reload server**

```bash
docker run -it --rm --name node-script -p 8080:8080 -v "$PWD":/usr/src/app -w /usr/src/app node:10.16.0-alpine npm i @vue/cli -g && vue create . && npm run serve
```

You can run it at [0.0.0.0:8080](http://0.0.0.0:8080/).


**2. Run the hot reload server**

```bash
docker run -it --rm --name node-script -p 8080:8080 -v "$PWD":/usr/src/app -w /usr/src/app node:10.16.0-alpine npm run serve
```

You can run it at [0.0.0.0:8080](http://0.0.0.0:8080/).


**3. Use custom commands (nodejs or other)**

```bash
docker run -it --rm --name node-script -p 8080:8080 -v "$PWD":/usr/src/app -w /usr/src/app node /bin/bash
# Write your custom command here like:
# npm run serve
# npm run lint
# npm run build
```

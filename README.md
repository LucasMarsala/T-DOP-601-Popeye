# Introduction

The aim of the project was to deploy a poll app using docker and docker-compose

![docker logo](https://d1.awsstatic.com/acs/characters/Logos/Docker-Logo_Horizontel_279x131.b8a5c41e56b77706656d61080f6a0217a3ba356d.png)

## Requirements

Docker - Docker-compose

```bash

sudo apt-get install docker docker-compose

```

To deploy the project, you need to create .env files at the root of each project.

### Poll .env content

REDIS_HOST=redis
</br>
PORT=80
</br>
HOST=0.0.0.0

### Worker .env content

DATABASE_HOST=db
</br>
POSTGRES_USER=postgres
</br>
POSTGRES_PASSWORD=password
</br>
POSTGRES_DB=postgres
</br>
REDIS_HOST=redis

### Result .env contents

DATABASE_HOST=db
</br>
POSTGRES_USER=postgres
</br>
POSTGRES_PASSWORD=password
</br>
POSTGRES_DB=postgres
</br>
PORT=80

### At the root of the T-DOP-600 folder

DATABASE_HOST=db
</br>
POSTGRES_USER=postgres
</br>
POSTGRES_PASSWORD=password
</br>
POSTGRES_DB=postgres
</br>
REDIS_HOST=redis



## Usage

```bash

docker-compose build

docker-compose --env-file .env up -d

```

# Introduction

The aim of the project was to deploy a poll app using docker and docker-compose

![docker logo](https://d1.awsstatic.com/acs/characters/Logos/Docker-Logo_Horizontel_279x131.b8a5c41e56b77706656d61080f6a0217a3ba356d.png)
![Screenshot_2023-03-21_11-16-52](https://user-images.githubusercontent.com/39527261/226577173-6d0d765e-31b8-4f8f-b707-b01483c5fc09.png)
![Screenshot_2023-03-21_11-17-17](https://user-images.githubusercontent.com/39527261/226577184-e3655aa1-ba06-48b7-87e1-e0fe9f3f43a2.png)

## Requirements

Docker - Docker-compose

```bash

sudo apt-get install docker docker-compose

```

To deploy the project, you need to create .env file.

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
</br>
PORT=80
</br>
HOST=0.0.0.0



## Usage

```bash

docker-compose build

docker-compose up -d

```

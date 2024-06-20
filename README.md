# Introduction

The aim of the project was to deploy a poll app using docker and compose

![docker logo](https://d1.awsstatic.com/acs/characters/Logos/Docker-Logo_Horizontel_279x131.b8a5c41e56b77706656d61080f6a0217a3ba356d.png)
![Screenshot_2023-03-21_11-16-52](https://user-images.githubusercontent.com/39527261/226577173-6d0d765e-31b8-4f8f-b707-b01483c5fc09.png)
![Screenshot_2023-03-21_11-17-17](https://user-images.githubusercontent.com/39527261/226577184-e3655aa1-ba06-48b7-87e1-e0fe9f3f43a2.png)

## Requirements

Docker version 20 >=

```bash

sudo apt-get install docker 

```

To deploy the project, you need to create .env file.

### At the root of the T-DOP-600 folder

```bash
POSTGRES_HOST=db
POSTGRES_PORT=5432
POSTGRES_USER=postgres
POSTGRES_PASSWORD=password
POSTGRES_DB=postgres
REDIS_HOST=redis
```


## Usage

```bash

docker compose build

docker compose up -d

```

# heroes
Docker Poetry Fastapi SQLModel Hello World

Esta app es un ejemplo de hola mundo usando:
* fastapi: https://fastapi.tiangolo.com/
* sqlmodel: https://sqlmodel.tiangolo.com/
* httpx: https://www.python-httpx.org/

Forma parte del ejemplo de como ejecutar un sistema de varias apps utilizando docker-compose y git submodule.
https://github.com/taller-de-programacion-2/integration

# Ejecución
Para ejecutar la app debemos pasar por envvar la url de la base sql y la url del servicio de users https://github.com/paulocesarcuneo/users.

```

DATABASE_URL=postgresql://postgres:postgres@localhost:5432/heroes USERS_HOST=http://localhost:8080/users poetry run uvicorn main:app --port 8081

```

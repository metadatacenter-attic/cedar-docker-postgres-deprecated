# cedar-docker-postgres
Postgres for Keycloak

The content is based on:

https://github.com/docker-library/postgres/tree/3d4e5e9f64124b72aa80f80e2635aff0545988c6/9.6

## Building and pushing to DockerHub:

````
chmod a+x docker-entrypoint.sh

docker build -t cedar-postgres .

docker login

docker tag cedar-postgres metadatacenter/cedar-postgres:0.1.0
docker push metadatacenter/cedar-postgres:0.1.0

docker tag cedar-postgres metadatacenter/cedar-postgres:latest
docker push metadatacenter/cedar-postgres:latest
````
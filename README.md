# Blog API

## Setup Database Container
To set up a local database image make sure docker is installed and running. Then execute the following command to download and run Postgres:

`docker run -itd --name postgres -e POSTGRES_PASSWORD=password -e POSTGRES_USER=brantunger -e POSTGRES_DB=blogdb -p 5432:5432 postgres`

On future restarts of your machine get the docker CONTAINER_ID then restart the container:
```
docker ps -a      
docker start CONTAINER_ID
```

To log in to the local database from a postgres client or GUI Database tool you can use the following credentials:
```
Username: brantunger
Password: password
```
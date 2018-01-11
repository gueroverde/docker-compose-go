# docker-compose-go
this is my docker test about to learn go
You have to have docker and docker compose installed 
Docker Engine release 1.13.0+
and docker-compose latest version

to use clone this repo in any path.
and run docker-compose up -d 

to verify is up the container run:

docker ps


And finally to enter the container:

```docker-compose exec -u gueroverde go bash ```

to run go tour 
```go tool tour -http 0.0.0.0:3999```

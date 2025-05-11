# globeco-order-service-postgresql
PostgreSQL database for the GlobeCo Order Service.



To build:

```
docker build -t kasbench/globeco-order-service-posgresql .
```

To run:

```
docker run -d --name globeco-order-service-postgresql \
  -p 5432:5432 \
  -e POSTGRES_HOST_AUTH_METHOD=trust \
  kasbench/globeco-order-service-posgresql
```

With network

```
docker run -d --name globeco-order-service-postgresql \
  -p 5432:5432 \
  -e POSTGRES_HOST_AUTH_METHOD=trust \
  --network my-network \
  kasbench/globeco-order-service-posgresql
```

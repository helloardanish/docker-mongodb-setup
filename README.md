### Host mongodb on your local in single click using docker compose

```
docker compose up # to run it
docker compose down # to stop it
```

### Access over the web using mongo-express

![image](https://github.com/user-attachments/assets/48ede922-594b-493e-b13a-89a4589736c9)

```
url: http://localhost:8081/

#Credentials
username: admin
password: pass


# same can be found in docker log
mongo-express  | Mongo Express server listening at http://0.0.0.0:8081
mongo-express  | Server is open to allow connections from anyone (0.0.0.0)
mongo-express  | basicAuth credentials are "admin:pass", it is recommended you change this in your config.js!
```

### If you want to use in spring boot application for some test

```
spring:
  data:
    mongodb:
      uri: mongodb://admin:system@localhost:27017/test-data?authSource=admin
```

Only database is required in spring mongodb configuration details. Here database is `test-data`

![image](https://github.com/user-attachments/assets/29da6d53-5c9a-4b37-a152-044fbab114c0)


### Create new database, read, write, modify, update using web or using backend services.

### Happy Coding,
## A R

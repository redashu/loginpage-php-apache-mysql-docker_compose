### mysql container images requirement --

```
MYSQL_USER: 
MYSQL_PASSWORD:
MYSQL_DATABASE:
```
### note : if you have mysql backup file then mount it given section 

```
datadb:
    container_name: db
    image: mysql
    volumes:
     - ./sql:/docker-entrypoint-initdb.d/
    restart: always
    environment:
        MYSQL_ROOT_PASSWORD: q1234
        MYSQL_DATABASE: login
        MYSQL_USER: akash
        MYSQL_PASSWORD: q1234

```


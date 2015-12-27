Create the image:

`docker build -t mysql_data .`

docker-compose.yml file:

```
...

db:
    image: mysql
    volumes_from:
        - mysql_data
mysql_data:
    image: mysql_data
```
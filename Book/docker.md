### Build image 
```bash
docker build -t wordpress-test-image .
```
### create container

```bash
docker run -p 8080:80 wordpress-test-image
```
```bash
docker run -d --name wordpress-test-image-container -p 8080:80 wordpress-test-image
```


```bash
docker exec -it wordpress-test-image-container /bin/bash
docker exec -u www-data -it wordpress-test-image-container bash
docker exec -it mysqldb /bin/bash

```


```bash
docker-compose up --build -d
docker-compose ps

docker-compose --verbose up --build | tee build.log


```



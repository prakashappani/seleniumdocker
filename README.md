# Selenium - Chrome image building
docker build --tag=myuitest .

## How to use this image

First, you will need a Selenium Grid Hub that the Node will connect to.

```
docker run -d -p 4444:4444 --name myuitest -v /dev/shm:/dev/shm  myuitest 
docker exec -it myuitest bash```

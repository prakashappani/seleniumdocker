## How to  get this project

Clone this repository
```
git clone https://github.com/prakashappani/seleniumdocker.git
```
## How to Build Selenium - Chrome docker image 
```
docker build --tag=myuitestsdockerimage .
```
## How to use this image

First, you will need a Selenium Grid Hub that the Node will connect to.

```
docker run -d -p 4444:4444 --name myuitestsdockercontainer -v /dev/shm:/dev/shm  myuitestsdockerimage 
docker exec -it myuitestsdockercontainer bash
```
## How to get latest code

OPTIONAL STEP: Pull the latest code.

```
git pull "https://github.com/prakashappani/swaglabsuitests.git" 
```

## How to run UI Tests

Run the Test Suite

```
grunt --conf=feature.filename --suite=Suite Name
grunt --conf=./TestModule_SWAGLABS/Conf/protractor.conf.js --suite=Regression
```

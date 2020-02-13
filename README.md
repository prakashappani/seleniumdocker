## How to Build Selenium - Chrome docker image 
```
docker build --tag=myuitest .
```
## How to use this image

First, you will need a Selenium Grid Hub that the Node will connect to.

```
docker run -d -p 4444:4444 --name myuitest -v /dev/shm:/dev/shm  myuitest 
docker exec -it myuitest bash
```
## How to get latest code

Pull the latest code.

```
git pull "https://github.com/prakashappani/swaglabsuitests.git" 
```

## How to run UI Tests

Run the Test Suite

```
grunt --conf=feature.filename --suite=Suite Name
grunt --conf=./TestModule_SWAGLABS/Conf/protractor.conf.js --suite=Regression
```

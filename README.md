# Setup local environment
## Method 1: via docker
- Start server:
```
cd docker
docker-compose build
docker-compose up
```
## Method 2: setup environment manually
# Setup server environment
Using pm2 as nodejs process manage
- install pm2 if not yet installed on system
```shell
npm install -g pm2
```  
- install pm2-logrotate to prevent disk full in the future
```shell
pm2 install pm2-logrotate
```
default config is OK
- start services
```shell
$ # cd to folder include ecosystem.config.js
$ pm2 start
```
# virus-homepage

## Usage

#### Install
```
$ npm install
```

#### Test on local
```
$ npm run dev
```
> http://0.0.0.0:8080 OR http://localhost:8080  

#### Release

###### Build
```
$ npm run build
```

## Install on server

#### Port settings

```
~$ cd /opt/bitnami
/opt/bitnami$ sudo ./ctlscript.sh stop apache
```

>> Add 'Custom - TCP - 3000' on lightsail - networking

#### Run

```
~/workspace/virus-homepage$ sudo npm start
~/workspace/virus-homepage$ sudo forever --minUptime 5 --spinSleepTime 5 start ./bin/www ~/workspace/virus-homepage
$ sudo forever list ~/workspace/virus-homepage$ sudo forever stop /root/virus-homepage/bin/www
```

###### Deploy
Upload all files in `dist` folder.

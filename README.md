[![unifi](https://badgen.net/badge/UniFi/8.0.7-ls218?list=|&icon=https://docs.golift.io/svg/ubiquiti_color.svg&color=0099ee "UniFi Products Supported")](https://www.ui.com/download/unifi/)

<p align="center">
  <img src="https://github.com/AzagraMac/UnifiDocker/blob/main/unifi-banner.png"
       width="700"/>
</p>

<p align="center">
  <img src="https://logos-world.net/wp-content/uploads/2021/02/Docker-Symbol.png" 
       width="300"/>
</p>

### Requeriments
- Service docker running

### Install 
`git clone https://github.com/AzagraMac/UnifiDocker.git`

### Deploy
```
cd UnifiDocker
docker-compose up -d
```
The first one to be deployed, you have to download the image and the Unifi package, you can monitor it from the logs command, wait at least 5 minutes (depending on the computer where you deploy it) before loading the web.

### Log
```
docker logs unifi-controller
```

#### Example log output
```
[migrations] started
[migrations] no migrations found
[cont-init.d] 01-migrations: exited 0.
[cont-init.d] 10-adduser: executing... 
usermod: no changes

-------------------------------------
          _         ()
         | |  ___   _    __
         | | / __| | |  /  \
         | | \__ \ | | | () |
         |_| |___/ |_|  \__/


Brought to you by linuxserver.io
-------------------------------------

To support LSIO projects visit:
https://www.linuxserver.io/donate/
-------------------------------------
GID/UID
-------------------------------------

User uid:    1000
User gid:    1000
-------------------------------------

[cont-init.d] 10-adduser: exited 0.
[cont-init.d] 15-install: executing... 
[cont-init.d] 15-install: exited 0.
[cont-init.d] 19-deprecate: executing... 
[cont-init.d] 19-deprecate: exited 0.
[cont-init.d] 20-config: executing... 
*** Setting Java memory limit to 1024 ***
*** Setting Java memory minimum to 1024 ***
[cont-init.d] 20-config: exited 0.
[cont-init.d] 30-keygen: executing... 
[cont-init.d] 30-keygen: exited 0.
[cont-init.d] 90-custom-folders: executing... 
[cont-init.d] 90-custom-folders: exited 0.
[cont-init.d] 99-custom-scripts: executing... 
[custom-init] no custom files found exiting...
[cont-init.d] 99-custom-scripts: exited 0.
[cont-init.d] done.
[services.d] starting services
[services.d] done.
...
```

### Access to the dasboard
Access to URL `https://IP_HOST:8443`

#### Configure it normally. 
<p align="center">
  <img src="https://github.com/AzagraMac/UnifiDocker/blob/main/cap01.png" />
</p>

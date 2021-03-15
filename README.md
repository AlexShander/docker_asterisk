Asterisk PBX Docker image + docker-compose file with macvlan
============================================================

The CentOS 7 base Docker image with Asterisk PBX 13.37.0 https://hub.docker.com/repository/docker/alexshander/asterisk

### How to use
```docker compose up -d```
### Notices
Yum must to change network settings to yours or magic could not work.
There are network settings in docker-compose.yml. I used for example network 192.168.14.0/24 and host is 192.168.14.16.

### What's missing

Only base Asterisk packages installed, without odbc or mysql, however you may install additional packages with `yum` command:

- asterisk-13.37.0 
- asterisk-sip-13.37.0
- asterisk-curl-13.37.0 
- asterisk-mp3-13.37.0
- asterisk-ael-13.37.0
- asterisk-lua-13.37.0 
- asterisk-sqlite-13.37.0 
- asterisk-voicemail-13.37.0
- asterisk-devel-13.37.0 
- asterisk-pjsip-13.37.0


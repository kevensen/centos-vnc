# centos-vnc
Installs tigervnc-server in a CentOS 6 based docker container.  This is the first container you should build.  Frankly, this doesn't do much.  What you should do is pull the docker.io/kevensen/centos-vnc-firefox image which uses this image.  The purpose is to decouple the application being run from the VNC server foundation.  

Or you can simply pull the image.
```
docker pull docker.io/kevensen/centos-vnc
```

##Instructions for Building
```
docker build -t centos-vnc .
```

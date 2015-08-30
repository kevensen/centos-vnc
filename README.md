# docker-rhel-vnc
Run Firefox inside a RHEL 6 based docker container.  This is the first container you should build.

##Instructions for Building
```
docker build -t rhel-vnc .
```

## Instructions for Running without Kubernetes

1.) Run the container and test the connection with your favorite VNC viewer.  The password is `basicuser`.
```
docker run -d -p 5901:5901 --name vnc rhel-vnc
```
2.) Stop and remove the container.
```
docker stop vnc
docker rm vnc
```
3.) Start the container in preparation for the XRDP container
```
docker run -d --name vnc registry.example.com:5000/rhel-vnc
```

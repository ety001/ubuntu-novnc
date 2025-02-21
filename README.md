# Ubuntu NoVNC Desktop

An Ubuntu 18.04 Desktop in a Docker container, running

* Xfce4
* Firefox
* Terminal

## Run the Container

`docker run -d -p 8080:8080 ety001/ubuntu-novnc`

## Access via Web Browser

`http://localhost:8080?password=insecure`

![](desktop1.png)

## Use a different Password

Make sure the password is 8 characters or less. VNC does not seem to like password that are too simple.

`docker run -d -p 8080:8080 -e vncpassword=hello123 ety001/ubuntu-novnc`

## Can I get 'classic VNC' as well?

Yes.

`docker run -d -p 5901:5901 ety001/ubuntu-novnc`

## Image on Docker Hub

[https://hub.docker.com/r/ety001/ubuntu-novnc](https://hub.docker.com/r/ety001/ubuntu-novnc)



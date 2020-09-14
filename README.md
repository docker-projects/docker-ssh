# alpine-ssh

Alpine Linux is a security-oriented, lightweight Linux distribution based on musl libc and busybox.

The above Dockerfile has root enabled in the ssh server as well as run ssh on the time of docker 
container creation.

# How to run the docker container with ssh ?

I have exposed the port 22 in the Dockerfile. You can use the below command to run the docker container.
```
docker run -d --name=ssh -p 7777:22 azagramac/alpine-ssh
```

To connect the docker container via ssh.
```
ssh root@localhost -p 7777
```
Password is: "EnterTheMatrix"


# Docker

Helpful tips for using docker:

## Manage Docker processes

```bash
$ docker ps     # show running docker proceeses
$ docker ps -a  # show all docker proceeses 
```

```bash
$ docker run <image:tag>       # run an image in foreground
$ docker run -d <image:tag>    # run an image in the background
$ docker run -it <image:tag>   # run an image in interactive tty mode
$ docker run -p <host:cntr>    # run an image publishing container ports to host
$ docker run --rm <image:tag>  # run an image and remove it on exit

### Example(s)
$ docker run -it --rm -d -p 8080:80 --name web nginx 
```

```bash
$ docker logs <container-id>     # fetch logs from a container
$ docker logs -f <container-id>  # fetch and follow logs from a container

$ docker attach <container-id>   # attach to a running container
```

```bash
$ docker stop <container-id>   # stop a running container
```

## List all of the currently cached images

```bash
$ docker images
$ docker images -a             # show all including intermediate images
```

## Remove a specific image

```bash
$ docker rmi <image-id>        # remove a specific image
$ docker rmi -f <image-id>     # force removal of an image
```

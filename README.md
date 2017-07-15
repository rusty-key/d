# d
Collection of shortcuts to make interactions with docker less painful

## Installing
Copy `d` to any directory of your `$PATH`. `/usr/local/bin` is a good place for `d`.

Or you can clone this repository whereever you want and add `/path/to/whereever/bin` to your `$PATH`.

## Usage

`d` - is simply an alias for `docker`:
```sh
d images
# the same as
docker image
```

More shortcuts:
```sh
# docker image
d i

# docker images
d is

# docker images -q
d isq

# docker images -a
d isa

# docker images -qa
d isqa

# docker ps
d l
d ls

# docker ps -a
d la

# docker ps -lq
d lq

# docker ps -laq
d laq

# docker build -t [name]
d b [name]

# docker exec -i -t [container] /bin/bash
d sh [container]

# docker rm $(docker images -q)
d rmi

# docker stop $(docker ps -laq)
d halt

# docker stop [container] && docker rm [container]
d rmf

# docker rm $(docker ps -laq)
d rmc

# docker stop $(docker ps -laq) && docker rm $(docker ps -laq)
d rmca

# docker run -d -P
d d

# docker volume
d v

# docker volume create --name [name]
d vc [name]

# d inspect --format '{{ .NetworkSettings.IPAddress }}'
d ip
```

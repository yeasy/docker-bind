Bind
===
Docker images for the bind dns server with web UI.


# Supported tags and respective Dockerfile links

* [`latest` (latest/Dockerfile)](https://github.com/yeasy/docker-bind/blob/master/Dockerfile)

For more information about this image and its history, please see the relevant manifest file in the [`yeasy/docker-bind` GitHub repo](https://github.com/yeasy/docker-bind).

# What is docker-bind?
Docker image with bind DNS server and web UI. The image is built based on [docker-bind](https://github.com/sameersbn/docker-bind).

# How to use this image?
The docker image is auto built at [https://registry.hub.docker.com/u/yeasy/bind/](https://registry.hub.docker.com/u/yeasy/bind/).


## In Dockerfile
```sh
FROM yeasy/bind:latest
```

## Local Run
After install [docker-compose](https://docs.docker.com/compose)
```sh
$ docker-compose up
```

# Which image is based on?
The image is based on `ubuntu:14.04`.

# What has been changed?

## add bind
Add the bind to listen on udp port 53.

## add web UI
Access port 10000 with root:password for access the web UI.

## disable unncessary task
Disable the daily apt-get update task.

# Supported Docker versions

This image is officially supported on Docker version 1.7.1.

Support for older versions (down to 1.0) is provided on a best-effort basis.

# User Feedback
## Documentation
Be sure to familiarize yourself with the [repository's `README.md`](https://github.com/yeasy/docker-bind/blob/master/README.md) file before attempting a pull request.

## Issues
If you have any problems with or questions about this image, please contact us through a [GitHub issue](https://github.com/yeasy/docker-bind/issues).

You can also reach many of the official image maintainers via the email.

## Contributing

You are invited to contribute new features, fixes, or updates, large or small; we are always thrilled to receive pull requests, and do our best to process them as fast as we can.

Before you start to code, we recommend discussing your plans through a [GitHub issue](https://github.com/yeasy/docker-bind/issues), especially for more ambitious contributions. This gives other contributors a chance to point you in the right direction, give you feedback on your design, and help you find out if someone else is working on the same thing.

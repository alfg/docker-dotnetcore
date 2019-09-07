# Docker dotnet core
> A Dockerfile installing and running a basic aspnet webapi app.

Use this as a template for running aspnet apps in Docker.

[![Docker Stars](https://img.shields.io/docker/stars/alfg/dotnetcore.svg)](https://hub.docker.com/r/alfg/dotnetcore/)
[![Docker Pulls](https://img.shields.io/docker/pulls/alfg/dotnetcore.svg)](https://hub.docker.com/r/alfg/dotnetcore/)
[![Docker Automated build](https://img.shields.io/docker/automated/alfg/dotnetcore.svg)](https://hub.docker.com/r/alfg/dotnetcore/builds/)
[![Build Status](https://travis-ci.org/alfg/docker-dotnetcore.svg?branch=master)](https://travis-ci.org/alfg/docker-dotnetcore)

## Usage
* Pull Docker image and run:
```
docker pull alfg/dotnetcore
docker run -it -p 8080:80 --rm alfg/dotnetcore
```

* or build and run container from source:
```
docker build -t dotnetcore
docker run -it -p 8080:80 --rm dotnetcore
```

```
$ curl localhost:8080/api/values

HTTP/1.1 200 OK
Date: Sat, 07 Sep 2019 04:13:22 GMT
Content-Type: application/json; charset=utf-8
Server: Kestrel
Transfer-Encoding: chunked

["value1","value2"]
```

## Resources
* https://hub.docker.com/_/microsoft-dotnet-core
* https://github.com/dotnet/dotnet-docker
* https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/docker

## License
MIT
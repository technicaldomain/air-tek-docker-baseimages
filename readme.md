# Docker base images

Implementation of [Docker base image](https://docs.docker.com/build/building/base-images/) concept

## [ASP.NET 5](./aspnet-5/)

Docker image to run applications based on ASP.NET 5

Configuration includes:

* non-root user
* automatic upgrade system to the latest package versions
* declaration default web-application port (8080)
* exposure port 8080 by default
* configuration default working directory
* providing default health check for web application

## [ASP.NET 6](./aspnet-6/)

Docker image to run applications based on ASP.NET 5

Configuration includes:

* non-root user
* declaration default web-application port (8080)
* exposure port 8080 by default
* configuration default working directory

## License
Apache 2 Licensed. For more information please see [LICENSE](./LICENSE)

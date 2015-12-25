Docker Build Files
----------------------

Just some Dockerfiles for a personal project. Nothing to see here. Move along.

#### ubuntu-base

Initially it was suggested to me to add `build-essential` to the base image but it pumps it up to ~700MB which I'm not so keen on. Let's see whether we really need it first, eh?

#### mongodb

*ISSUES:*
Currently unable to disable [transparent huge pages](https://docs.mongodb.org/master/tutorial/transparent-huge-pages/) in the Ubuntu kernel.

#### buildpack-deps

A version of [buildpack-deps](https://hub.docker.com/r/library/buildpack-deps/) based upon [wily-scm](https://github.com/docker-library/buildpack-deps/blob/1845b3f918f69b4c97912b0d4d68a5658458e84f/wily/scm/Dockerfile) and [wily](https://github.com/docker-library/buildpack-deps/blob/ca0f463579583f030cb5c8eb2c8dac207709feb5/wily/Dockerfile) collapsed into one image and based upon my own Ubuntu 16.04 base image.

Build with:

	docker build -t garethmj/buildpack-deps:16.04 .

#### NodeJS

A version of [Node Official](https://hub.docker.com/_/node/) but based upon my own Ubuntu 16.04 buildpack-deps.

Build with:

	docker build -t garethmj/node:5.3.0 .

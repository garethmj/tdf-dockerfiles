Docker Build Files
----------------------

Just some Dockerfiles for a personal project. Nothing to see here. Move along.

#### ubuntu-base

Initially it was suggested to me to add `build-essential` to the base image but it pumps it up to ~700MB which I'm not so keen on. Let's see whether we really need it first, eh?

#### mongodb

*ISSUES:*
Currently unable to disable [transparent huge pages](https://docs.mongodb.org/master/tutorial/transparent-huge-pages/) in the Ubuntu kernel.

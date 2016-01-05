# taiga-environment
Complete taige-environment

This repo contains the build files for a docker image to run a hole taiga-environment.

https://taiga.io/ is a project management platform for startups and agile developers & designers who want a simple, beautiful tool that makes work truly enjoyable.

This Docker image can be used for running a complete Taiga Environment (Postgresql + Taiga-Back- and Frontend ).


WARNING: It's under development.


Including:

-postgresql
-taiga-backend
-taiga-frontend

Dockhub: https://hub.docker.com/r/bitstrange/taiga/


Command to start container: 

docker run --name taiga -d \
      -v PATH/local.py:/home/taiga/taiga-back/settings/local.py \
      -v PATH/conf.json:/home/taiga/taiga-front-dist/dist/js/conf.json \
      -p 80:80 bitstrange/taiga:latest

You will habe to provide the files 

local.py

and

conf.json


You will find these files in the "volume" directory of this repo.



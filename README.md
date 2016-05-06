# taiga-environment
Complete Taiga environment

Dockhub: https://hub.docker.com/r/jcpw/taiga-environment/
Github: https://github.com/jimeney/taiga-environment

https://taiga.io/ is a project management platform for startups and agile developers & designers who want a simple, beautiful tool that makes work truly enjoyable.

This is a self-contained docker image Including:

-postgresql
-taiga-backend
-taiga-frontend

It is based on the original work here on the Docker Hub:
https://hub.docker.com/r/bitstrange/taiga/


Command to start container: 

docker run --name taiga -d \
-v PATH/local.py:/home/taiga/taiga-back/settings/local.py \
-v PATH/conf.json:/home/taiga/taiga-front-dist/dist/js/conf.json \
-v PATH/app-loader.js:/home/taiga/taiga-front-dist/dist/v-1461931321319/js/app-loader.js \
-p 80:80 jcpw/taiga-environment:latest

You will have to provide the files 

local.py - set up Email, the URI etc.
conf.json - set up the URI to the API
app-loader.js - set up the URI to the API

It’s a work in progress, based on the STABLE branch of TAIGA, the image was built on 6th May 2016


You will find these files in the "volume" directory of this repository.
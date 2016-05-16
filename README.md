# taiga-environment
Complete Taiga Environment

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

docker run --name taiga -d -p 80:80 jcpw/taiga-environment:latest

You will have to provide the following environment variables for it to work: 

SITE_URI
ADMIN_EMAIL
NOREPLY_EMAIL

Optionally, for emailing to work:
EMAIL_HOST
EMAIL_HOST_USER
EMAIL_HOST_PASSWORD
EMAIL_HOST_PORT
EMAIL_USE_TLS
EMAIL_BACKEND

It’s a work in progress, based on the STABLE branch of TAIGA, the image was built on 6th May 2016


You will find these files in the "volume" directory of this repository.
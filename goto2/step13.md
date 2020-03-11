First, let us build the Docker image...

`docker build . -t monolithclient`{{execute}}

Now, let's run it...

`docker run -p 8080:8080 monolithclient &`{{execute}}

Let's take a look at the web application...

Render port 8080: https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/
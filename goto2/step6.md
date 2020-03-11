First, let us build the Docker image...

`docker build . -t monolithserver`{{execute}}

Now, let's run it...

`docker run -p 9000:9000 monolithserver`{{execute}}

Let's take a look at the REST endpoints...

Render port 9000: https://[[HOST_SUBDOMAIN]]-9000-[[KATACODA_HOST]].environments.katacoda.com/
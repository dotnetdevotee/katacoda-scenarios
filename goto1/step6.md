Forward this to the other terminal...

`socat -d tcp-listen:9000,reuseaddr,fork tcp:[[HOST_SUBDOMAIN]]-9000-[[KATACODA_HOST]].environments.katacoda.com:80`{{execute}}

Now let's get the code...

`git clone https://github.com/mattjonesorg/DMRTechnology.git`{{execute}}


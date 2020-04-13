Now we need to edit the server URL ...

`apt update`{{execute}}

`apt install nano`{{execute}}

`cd DMRTechnology`{{execute}}

`cd client`{{execute}}

`cd src`{{execute}}

`cd services`{{execute}}

`nano server.js`{{execute}}

Now replace 'http://localhost:9000' with 'https://[[HOST_SUBDOMAIN]]-9000-[[KATACODA_HOST]].environments.katacoda.com'

Then hit CTRL-X and follow the prompts to save the file
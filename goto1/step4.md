Now we'll run the server...

`cd DMRTechnology`{{execute}}

`cd server`{{execute}}

`mvn org.springframework.boot:spring-boot-maven-plugin:run &`{{execute}}

`ssh localhost -L 8081: localhost:8080`{{execute}}

And now you can access the application here (in http)...

Render port 8080: https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/

Render port 8082: https://[[HOST_SUBDOMAIN]]-8082-[[KATACODA_HOST]].environments.katacoda.com/

Render port 80: https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com/

Display page allowing user to select port:
https://[[HOST_SUBDOMAIN]]-[[KATACODA_HOST]].environments.katacoda.com/
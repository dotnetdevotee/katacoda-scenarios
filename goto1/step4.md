Now we'll run the server...

`cd DMRTechnology`{{execute}}

`cd server`{{execute}}

`mvn org.springframework.boot:spring-boot-maven-plugin:run &`{{execute}}

Wait until you see a line in the console that says something like this: "StartedCalendarAppApplication in XXX seconds (JVM running for YYY)"

Let's take a look at the REST endpoints...

Render port 9000: https://[[HOST_SUBDOMAIN]]-9000-[[KATACODA_HOST]].environments.katacoda.com/api/auth/signin

<i>It is normal for this page to return an error, but we want to make sure it is the <b>right</b> error.  The final line should say: "Request method 'GET' not supported"</i>
Last, but not least, we want to tell Docker to start our server via Maven whenever we run our Docker image.  We do this using an ENTRYPOINT

<pre class="file" data-filename="Dockerfile" data-target="replace">
# We'll put our code here

FROM maven:3.6.3-jdk-11-openj9
COPY . .
ENTRYPOINT mvn org.springframework.boot:spring-boot-maven-plugin:run

</pre>
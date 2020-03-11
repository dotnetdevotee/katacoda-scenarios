We are going to run our server's maven target when we start our Docker image.  But, in order for that to work, we must tell it to begin in the directory where our POM file is located.

<pre class="file" data-filename="Dockerfile" data-target="replace">
# We'll put our code here

FROM maven:3.6.3-jdk-11-openj9
COPY server/ .
WORKDIR server

</pre>
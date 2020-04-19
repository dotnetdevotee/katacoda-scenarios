In our previous demo, we added "git" to our image and cloned down our code.

In a Dockerfile, we can simply tell Docker to copy all the files from our local directory onto the image as a part of the build.

<pre class="file" data-filename="Dockerfile" data-target="replace">
# We'll put our code here

FROM node:erbium-slim
COPY . .

</pre>
Last, but not least, we want to tell Docker to start our client via Yarn whenever we run our Docker image.  We do this using an ENTRYPOINT

<pre class="file" data-filename="Dockerfile" data-target="replace">
# We'll put our code here

FROM node:erbium-slim
COPY . .
RUN npm install
ENTRYPOINT yarn serve

</pre>
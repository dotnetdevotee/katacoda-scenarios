Now that our code will be in place on the Docker image, we need to run npm install in order to make sure all the right libraries are installed for run time execution.

<pre class="file" data-filename="Dockerfile" data-target="replace">
# We'll put our code here

FROM node:erbium-slim
COPY . .
RUN npm install

</pre>
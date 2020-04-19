Now, please navigate back up to the "client" directory in the Editor window and open the Dockerfile.  Then continue...

Let's start off by adding the base image for our Docker...

<pre class="file" data-filename="Dockerfile" data-target="replace">
# We'll put our code here

FROM node:erbium-slim

</pre>

If you did this correctly, you should now see code in your client Dockerfile to start a Dockerfile based on "node:erbium"
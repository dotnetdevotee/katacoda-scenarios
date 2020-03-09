<pre class="file" data-filename="app.js" data-target="replace">var http = require('http');
var requestListener = function (req, res) {
  res.writeHead(200);
  res.end('Hello, World!');
}

var server = http.createServer(requestListener);
server.listen(3000, function() { console.log("Listening on port 3000")});
</pre>

`ssh localhost -L 8081: localhost:8080`{{execute}}


Render port 8082: https://[[HOST_SUBDOMAIN]]-8082-[[KATACODA_HOST]].environments.katacoda.com/

Render port 80: https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com/

Display page allowing user to select port:
https://[[HOST_SUBDOMAIN]]-[[KATACODA_HOST]].environments.katacoda.com/


netcat -k -l -p 8082 -c "nc localhost 8080" &
socat tcp-listen:8081,reuseaddr,fork tcp:localhost:8080 &

socat -d tcp-listen:8084,reuseaddr,fork tcp:localhost:8080
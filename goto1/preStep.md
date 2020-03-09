First, we need to install Node...

`curl -sL https://deb.nodesource.com/setup_10.x | bash -`{{execute}}

`apt install -y nodejs`{{execute}}

`npm install -g yarn`{{execute}}

`netcat -l -p 8082 -c "nc localhost 8080" &`{{execute}}

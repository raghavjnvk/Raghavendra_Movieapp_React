sudo npm install -g eslint
sudo npx json-server --watch data.json

sudo npm cache clear --force
sudo npm install 
sudo npm start

Note:
First, you would want to know which process is using port 3000
sudo lsof -i :3000
this will list all PID listening on this port, once you have the PID you can terminate it with the following:
kill -9 {PID}

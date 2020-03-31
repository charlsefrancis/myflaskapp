# myflaskapp

Download the myflaskapp
Then start the Docker server environment 

Run the following to list any running images:

docker-compose images


Container    Repository     Tag       Image Id      Size
---------------------------------------------------------
flask       docker_flask   latest   d7ea63adcedf   899 MB
nginx       docker_nginx   latest   8b3031c24599   104 MB


docker-compose ps will list any running containers:

docker-compose ps


Name          Command          State         Ports
---------------------------------------------------------
flask   uwsgi app.ini          Up      8080/tcp
nginx   nginx -g daemon off;   Up      0.0.0.0:80->80/tcp


To stop our services:

docker-compose stop


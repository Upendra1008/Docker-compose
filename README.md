# Docker-compose-LAB
docker compose LAB for voting Application

## Docker-compose
Docker Compose is a tool that lets you define and run multi-container Docker applications using a single configuration file. 
Instead of running many docker run commands manually, you describe everything in a YAML file (docker-compose.yml) and start all containers together with one command. 

# STEPS for LAB
## Verify if docker compose is installed : docker-compose --version 
```
docker-compose --version
```
## If docker compose is not installed , install manually 
```
curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose 
```
## provide permission 
```
sudo chmod +x /usr/local/bin/docker-compose
```
## Create a Directory for  voting-app
```
mkdir voting-app 
cd voting-app 
```
## Create docker-compose.yml 
```
vi docker-compose.yml
check and copy the Docker-compose.yml file - 
```
## start the application with docker compose file 
run it in detach mode
```
docker-compose up –d 
```
## Verify the application in browser 
```
Open the Voting app with : http://<your EC2 public ip>:8080
Open the Voting result app with : http://<your EC2 public ip>:8081
```
## To  stop the entire application 
```
docker-compose down
```
## To remove all the stopped coinatiners 
```
review the stooped conatiners : docker ps -a
docker container prune
review if all the conatiners are deleted :  docker ps -a
```

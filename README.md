# Monitoring
Aim: Deploy a user-interactive application on Nginx along with Prometheus, Loki, and Grafana for monitoring and visualization

Step1- Update the system and install Docker and Docker Compose
sudo apt update && sudo apt upgrade -y
sudo apt install -y docker.io docker-compose
sudo usermod -aG docker $USER
newgrp docker

Step2- 
mkdir project && cd project
Create a docker-compose.yml file:
Create a prometheus.yml file inside ~/project/prometheus:
Create a local-config.yaml file inside ~/project/loki
Create an app directory and add a index.html file for the application

Step3-
docker-compose up -d
docker ps



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

Step 4: Configure Grafana for Monitoring
Login to Grafana:

Default username: admin
Default password: admin
Add Data Sources:

Prometheus:
Navigate to Configuration > Data Sources.
Select Prometheus and add http://prometheus:9090 as the URL.
Loki:
Add another data source and select Loki.
Set the URL to http://loki:3100.
Create Dashboards:

Use built-in templates or import JSON for Prometheus and Loki dashboards.


![Alt Text](/Images/monitoring.png)

# docker-compose

# Pre-requisites:
  - Install Java
  - Install Maven
  - Install Docker
  - Docker Swarm Setup
 
# Docker Swarm SetUp
  [Docker-Swarm](https://github.com/Naresh240/docker-swarm-setup.git)
# Create Docker Swarm master as jenkins slave
  ![Docker-Swarm-As-Jenkins-Slave](https://github.com/Naresh240/Jenkins-Master-Slave.git)
# Jenkins docker swarm deploy
  Create jenkins jobs with Jenkinsfile content and click on build
# Use postman app and Add Employee data
Check API: /addEmployee

    http://<ip-address>:8080/addEmployee
  
In postman app keep Post method and give Json data by selecting Body --> raw (Json format)

    {"id": "1001", "name": "Naresh", "departement": "Engineer"}
    
Check API:- /findAllEmployees

Goto Web UI and check below link

    http://<ip-address>:8080/findAllEmployees
# CleanUP
    docker stop <container-name>
    docker rm <container-name>
    
# Deploy springboot-mongodb application using docker-compose
    docker-compose up -d
# Use postman app and Add Employee data

Check API: /addEmployee

    http://<ip-address>:8080/addEmployee
  
In postman app keep Post method and give Json data by selecting Body --> raw (Json format)

    {"id": "1001", "name": "Naresh", "departement": "Engineer"}
    
Check API:- /findAllEmployees

Goto Web UI and check below link

    http://<ip-address>:8080/findAllEmployees
    
# To down our springboot-mongodb application
    docker-compose down

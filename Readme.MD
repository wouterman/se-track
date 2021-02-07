# Jenkins
This repository contains a docker-compose file to run a Jenkins instance in a container using Docker. The folder jenkins/jenkins_home is used to persist data.
The container has Maven, Java 11 and access to the Docker daemon of the host machine.

## How to run
Run the following two commands from the jenkins directory:
```
docker-compose build
docker-compose up -d
```

Check the Jenkins logs with:
```
docker logs jenkins
```

If you see the following line everything is good:
> *hudson.WebAppMain$3#run: Jenkins is fully up and running*


Access Jenkins at [http://localhost:3080](http://localhost:3080)  
Note that the port is __3080__.  
Login: admin/admin

Run the 'tools-test' job to verify that all tools are accessible.

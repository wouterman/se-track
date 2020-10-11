# Jenkins
Runs a Jenkins container in Docker using the folder jenkins_home to persist data.
The container has Maven, Java 11 pre-installed and access to the Docker daemon of the host machine.

## How to run
Run the following two commands:
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


Access jenkins at [http://localhost:3080](http://localhost:3080)

Login: admin/admin

Run the 'tools-test' job to verify that all tools are accessible.
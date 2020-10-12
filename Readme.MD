# CICD, Kubernetes and Microservices

## Recommended Courses on Pluralsight
* [Microservices: Getting started](https://www.pluralsight.com/courses/getting-started-microservices)
* [Docker and Kubernetes the big picture](https://www.pluralsight.com/courses/docker-kubernetes-big-picture)
* [Clean architecture: Patterns, Practices and Principles](https://www.pluralsight.com/courses/clean-architecture-patterns-practices-principles)
* [Kubernetes for Developers: Core Concepts](https://www.pluralsight.com/courses/kubernetes-developers-core-concepts)
* [DevOps: The Big Picture](https://www.pluralsight.com/courses/devops-big-picture)
* [Test Driven Development: The Big Picture](https://www.pluralsight.com/courses/test-driven-development-big-picture)
* [Continuous Integration and Continuous Delivery: The Big Picture](https://www.pluralsight.com/courses/continuous-integration-delivery-big-picture)

## Assignments

### Docker
* Install [Docker Desktop](https://docs.docker.com/docker-for-windows/install/)
* Dockerize your application via Dockerfile.
* Replace H2-file with database container (Postgres, MySQL, ....)
* Generate any necessary test-data on startup via you @Configuration-class
* Add a docker-compose file to quickly test your application in a production-like environment.

### CICD
* Use Jenkins to build and test you application on every push.
* Push the docker image, in the Maven deploy-phase, to your local registry.
* Start your container from Jenkins.
* Use a Jenkins Pipeline to script the different 'stages' of your build.
* Add the Pipeline script as a Jenkinsfile to your source repository.
* Bonus: Add unit tests and visualize these in Jenkins.

### Kubernetes
* Add Kubernetes deployment descriptors (Deployment, Service, ...) and add these to source control.
* Deploy from your pipeline to your local Kubernetes cluster.
* Bonus: Inject the database credentials via Kubernetes Secret.

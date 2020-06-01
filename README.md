### Spring Boot-Jenkins-Heroku demo 
Spring Boot app released on Heroku using local Docker Jenkins environment. Stub project.

### Configuration
- configure paths to volumes in `/docker/jenkins/jenkins.yml`
- start docker compose `docker-compose -f docker/jenkins/jenkins.yml up -d`
- install all Jenkins addons and configure user
- create a Jenkins job based on the `/Dockerfile` taken from repository
- configure Maven in Jenkins - it's name should be the same as the name defined in `Dockerfile` 
- to let Jenkins deploy app on Heroku, local system variable called HEROKU_API_KEY should be defined in Jenkins. Value should be taken from the Heroku profile.


### start jenkins using docker-compose
`docker-compose -f docker/jenkins/jenkins.yml up -d`

Docker is up on:
    
    http://192.168.99.100:8080/





